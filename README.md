# GTECH785_Fall22
 
Assignments for Hunter College GTECH 78519 Geospatial Databases, Fall 2022.<br>

SQL code and screenshots for Lab 2 <br>

SQL Code for Question 1: <br>
```sql
CREATE TABLE payment_bk AS
SELECT *
FROM payment;
```
<br>Result: <br>

![Lab 2, Q1 Result](image/L2Q1.png)

<br>SQL Code for Question 2: <br>
```sql
ALTER TABLE payment 
ADD COLUMN refund money;
UPDATE payment
SET refund = amount * .05
WHERE amount > 5.00;
```
<br>Result: <br>

![Lab 2, Q2 Result](image/L2Q2.png)

<br> SQL Code for Question 3: <br>
```sql
ALTER TABLE payment
ADD COLUMN is_refunded boolean;
UPDATE payment
SET is_refunded = TRUE
WHERE refund IS NOT NULL
UPDATE payment
SET is_refunded = FALSE
WHERE refund IS NULL;

CREATE VIEW payment_1 AS 
SELECT * FROM payment;
```
<br>Result: <br>

![Lab 2, Q3 Result](image/L2Q3.png)

<br> SQL Code for Question 4: <br>
```sql
CREATE TABLE customer_contact AS
SELECT first_name || ' ' || last_name as full_name, customer.address_id, address.address, address.postal_code, city.city, country.country
FROM customer
LEFT JOIN address ON address.address_id = customer.address_id
LEFT JOIN city ON address.city_id = city.city_id
LEFT JOIN country ON city.country_id = country.country_id ;
```
<br>Result: <br>

![Lab 2, Q4 Result](image/L2Q4.png)

<br> SQL Code for Question 5: <br>
```sql
CREATE TABLE customer_payment AS
SELECT first_name || ' ' || last_name as full_name, payment.amount
FROM customer
LEFT JOIN payment ON customer.customer_id = payment.customer_id;

SELECT full_name, sum(amount) total
FROM customer_payment
GROUP BY full_name
ORDER BY total desc
LIMIT 10;
```
<br>Result: <br>

![Lab 2, Q5 Result](image/L2Q5.png)

