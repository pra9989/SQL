The SQL AND Operator
The WHERE clause can contain one or many AND operators.

The AND operator is used to filter records based on more than one condition.
Note: The AND operator displays a record if all the conditions are TRUE.

The following SQL selects all customers from Spain that starts with the letter 'G':

ExampleGet your own SQL Server
Select all customers where Country is "Spain" AND CustomerName starts with the letter 'G':
SELECT *
FROM Customers
WHERE Country = 'Spain' AND CustomerName LIKE 'G%'; 
it will filter the customer name which are starting with G in spain country

AND Syntax
SELECT column1, column2, ...
FROM table_name
WHERE condition1 AND condition2 AND condition3 ...;

All Conditions Must Be True
The following SQL selects all customers where Country is "Brazil" AND City is "Rio de Janeiro" AND CustomerID is higher than 50:
SELECT * FROM Customers
WHERE Country = 'Brazil'
AND City = 'Rio de Janeiro'
AND CustomerID > 50;

AND vs. OR
The AND operator displays a record if all the conditions are TRUE.
The OR operator displays a record if any of the conditions are TRUE.

Combining AND and OR
You can also combine AND and OR operators.
The following SQL selects all customers from Spain that starts with a "G" or an "R" (make sure to use parenthesis to get the correct result):

Example
Select all Spanish customers that starts with either "G" or "R":
SELECT * FROM Customers
WHERE Country = 'Spain' AND (CustomerName LIKE 'G%' OR CustomerName LIKE 'R%');

Without parenthesis, the SQL above will return all customers from Spain that starts with a "G", plus all customers that starts with an "R", regardless of the country value:
Example:
SELECT * FROM Customers
WHERE Country = 'Spain' AND CustomerName LIKE 'G%' OR CustomerName LIKE 'R%';


