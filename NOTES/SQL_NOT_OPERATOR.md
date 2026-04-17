The NOT operator is used in the WHERE clause to return all records that DO NOT match the specified criteria. It reverses the result of a condition from true to false and vice-versa.
The following SQL selects all customers that are NOT from Spain:
SELECT * FROM Customers
WHERE NOT Country = 'Spain';
Select customers that does not start with the letter 'A':
SELECT * FROM Customers
WHERE CustomerName NOT LIKE 'A%';
The NOT BETWEEN Operator
SELECT * FROM Customers
WHERE CustomerID NOT BETWEEN 10 AND 60;
The NOT IN Operator
SELECT * FROM Customers
WHERE City NOT IN ('Paris', 'London');
NOT Greater Than
SELECT * FROM Customers
WHERE NOT CustomerID > 50;
NOT Less Than

SELECT * FROM Customers
WHERE NOT CustomerId < 50;



