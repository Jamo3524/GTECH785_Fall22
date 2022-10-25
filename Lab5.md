# GTECH785_Fall22

<b>SQL code and screenshots for Lab 5 </b><br>

<br>SQL Code for Task 1: <br>
```sql
--Creating a NY Pluto table
CREATE TABLE nypluto AS 
SELECT gid, zipcode, ownertype, yearbuilt, assesstot::money, geom
FROM mappluto;

--Creating a Queens Pluto table
CREATE TABLE qnspluto AS 
SELECT gid, zipcode, ownertype, yearbuilt, assesstot::money, geom
FROM mappluto
WHERE borough = 'QN';
```
Result:<br>
![Lab 5, Task 1 Result](image/L5Q1.PNG)

<br>SQL Code for Task 2: <br>
```sql
--Checking the SRIDs of the geometry columns
SELECT ST_SRID(geom_utm)
FROM ny_counties;
SELECT ST_SRID(geom)
FROM mappluto;

--Displaying the basemaps under the county and pluto data.
SELECT ST_Transform(geom, 4326) 
FROM ny_counties
LIMIT 100;
SELECT ST_Transform(geom, 4326) 
FROM qnspluto
LIMIT 300;

--Creating spatial indicies
CREATE INDEX pluto_geom_id
ON qnspluto
USING GIST (geom);
CREATE INDEX geom_id
ON ny_counties
USING GIST (geom_utm);

--Checking for simple and valid polygons
--All polygons in both shapefiles are simple and valid
SELECT *
FROM qnspluto
WHERE not ST_IsSimple(geom) or not ST_IsValid(geom);
SELECT *
FROM ny_counties
WHERE not ST_IsSimple(geom_utm) or not ST_IsValid(geom_utm);

--Changing the year built value to NULL for buildings listed being built in year 0
UPDATE qnspluto
SET yearbuilt = NULL
WHERE yearbuilt = 0;

--Setting the zipcode as NULL where zipcode = 0
UPDATE qnspluto
SET zipcode = NULL
WHERE zipcode = 0;

--Determining the percentage of properties with invalid zipcode or year built
--About 3.8% of properties had an invalid value for yearbuilt
--About 0.06% of properties had an invalid value for zipcode
SELECT
(SELECT count(*)
FROM qnspluto
WHERE yearbuilt IS NULL)::float/
(SELECT count(*)
FROM qnspluto)::float;
SELECT
(SELECT count(*)
FROM qnspluto
WHERE zipcode IS NULL)::float/
(SELECT count(*)
FROM qnspluto)::float;
```

Results:<br>
![Lab 5, Task 2 Result 1](image/L5Q2.PNG)
![Lab 5, Task 2 Result 1](image/L5Q3.PNG)
![Lab 5, Task 2 Result 1](image/L5Q4.PNG)
![Lab 5, Task 2 Result 1](image/L5Q5.PNG)

<br>SQL Code for Question 2.3: <br>
```sql
--Adding a geometry column to the NY Counties shapefile
ALTER TABLE ny_counties 
ADD COLUMN geom_utm geometry;

--Setting the new geometry column to UTM Zone 18N
UPDATE ny_counties
SET geom_utm = ST_Transform(geom, 3725);

--Confirming that the new column is in UTM Zone 18N
SELECT ST_SRID(geom_utm)
FROM ny_counties;

--Projecting on the fly to WGS 84 to view the basemap and verify the data
SELECT *, ST_Transform(geom_utm, 4326) AS temp_geom_wgs
FROM ny_counties;

```

Result:<br>
![Lab 4, Task 2.3 Result 3](image/L4Q2_3_1.PNG)

![Lab 4, Task 2.3 Result 2](image/L4Q2_3_2.PNG)

![Lab 4, Task 2.3 Result 1](image/L4Q2_3.png)

<br>SQL Code for Question 2.4: <br>
```sql
--Creating a spatial index for the NY Counties shapefile
CREATE INDEX ny_geom_id
ON ny_counties
USING GIST (geom_utm);
```

Result:<br>
![Lab 4, Task 2.3 Result](image/L4Q2_4.png)
