# GTECH785_Fall22
 
Assignments for Hunter College GTECH 78519 Geospatial Databases, Fall 2022.<br>

SQL code and screenshots for Lab 2 <br>

SQL Code for Question 1: <br>
```sql
CREATE TABLE payment_bk AS
SELECT *
FROM payment;
```

<br>SQL Code for Question 2: <br>
```sql
ALTER TABLE payment 
ADD COLUMN refund money;
UPDATE payment
SET refund = amount * .05
WHERE amount > 5.00;
```
