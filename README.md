# sql-intro-1

Answer the following questions using the SQL Fiddle here: https://www.db-fiddle.com/f/8aebs45GPaJUBgFNDuB1Rh/0

- 1.1 Select the names of all the products in the store.

Select Name from Products

- 1.2 Select the names and the prices of all the products in the store.

Select Name, Price from Products

- 1.3 Select the name of the products with a price less than or equal to $200.

Select Name from Products WHERE price <= 200

- 1.4 Select all the products with a price between $60 and $120.

Select Name from Products WHERE price >= 60 AND price <=120

- 1.5 Select the name and price in cents (i.e., the price must be multiplied by 100).

Select Name, Price*100 from Products 

- 1.6 Compute the average price of all the products.

Select AVG(Price) from Products 

- 1.7 Compute the average price of all products with manufacturer code equal to 2.

Select AVG(Price) from Products WHERE Manufacturer =2

- 1.8 Compute the number of products with a price larger than or equal to $180.

Select * from Products WHERE Price >= 180

- 1.9 Select the name and price of all products with a price larger than or equal to $180, and sort first by price (in descending order), and then by name (in ascending order).

Select Name,Price from Products WHERE Price >= 180 ORDER BY price DESC , Name ASC

- 1.10 Select all the data from the products, including all the data for each product's manufacturer.

Select * from Products INNER JOIN Manufacturers ON Products.Code = Manufacturers.Code

- 1.11 Select the product name, price, and manufacturer name of all the products.

Select Name, Price, Manufacturer from Products

