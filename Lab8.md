# GTECH785_Fall22

<b>SQL code and screenshots for Lab 8 </b><br>

<br>SQL Code for Task 1: <br>
```sql
--I loaded the block group shapefile into QGIS, the SRID is EPSG 4269, NAD 83
--Setting the SRID as 4269 and confirming it looks OK
CREATE TABLE nybg AS 
SELECT * FROM cb_2017_36_bg_500k;
SELECT UpdateGeometrySRID('nybg', 'geom', 4269);
SELECT Find_SRID('public', 'nybg', 'geom');
SELECT ST_Transform(geom, 4326) FROM nybg;

--Setting the geoid column to numeric, to match the education table
ALTER TABLE nybg
ALTER COLUMN geoid TYPE numeric USING geoid::numeric;

SELECT geoid::numeric
FROM nybg;

--Creating a spatial index on the block group table
CREATE INDEX bg_geom_index
ON nybg
USING GIST (geom);

--Calculating the total population with a bachelor's degree or higher
ALTER TABLE qns_ed
ADD COLUMN bach_higher numeric;
UPDATE qns_ed
SET bach_higher = bachelors + masters + professional + doctorate;

--Joining the Queens education table to the NY block group table
CREATE TABLE qnsed_geo AS
SELECT q.*, bg.affgeoid, bg.geom, bg.aland, bg.gid
FROM qns_ed as q
JOIN nybg as bg
ON q.geoid = bg.affgeoid;

--Displaying the Queens block groups on the basemap
SELECT ST_Transform(geom, 4326)
FROM qnsed_geo;
```
Results:<br>
![Lab 8, Task 1 Result 1](image/L8Q1.PNG)

<br>SQL Code for Task 2: <br>
```sql
--Setting the SRID of the subway stations shapefile
SELECT UpdateGeometrySRID('subwaystations', 'geom', 4326);
SELECT Find_SRID('public', 'subwaystations', 'geom');

--Finding the 5 closest fast food restaurants from each subway station
SELECT s.name, s.gid, rs.geom <-> s.geom dist, rs.name
FROM subwaystations s
CROSS JOIN LATERAL
(
SELECT r.id, r.name, r.geom
FROM restaurant_geom_geog1 r 
ORDER BY s.geom <-> r.geom
LIMIT 5
) AS rs;
```

Results:<br>
![Lab 6, Task 2 Result 1](image/L7Q3.PNG)



