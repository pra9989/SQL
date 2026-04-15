The SQL SELECT DISTINCT Statement
The SELECT DISTINCT statement is used to return only distinct (unique) values.

In a table, a column may contain several duplicate values - and sometimes you want to list only the unique values.
SELECT DISTINCT Country FROM Customers;

SELECT DISTINCT Syntax
SELECT DISTINCT column1, column2, ...
FROM table_name;

SELECT Example Without DISTINCT

If you omit the DISTINCT keyword, the SQL statement returns the "Country" value from all the records of the "Customers" table:
SELECT Country FROM Customers;
