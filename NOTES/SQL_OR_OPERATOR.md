SELECT *
FROM Customers
WHERE Country = 'Germany' OR Country = 'Spain';
Combining AND and OR
SELECT * FROM Customers
WHERE City = 'Berlin' OR CustomerName LIKE 'G%' OR Country = 'Norway';

SELECT * FROM Customers
WHERE Country = 'Spain' AND (CustomerName LIKE 'G%' OR CustomerName LIKE 'R%');

Without parenthesis, the SQL above will return all customers from Spain that starts with a "G", plus all customers that starts with an "R", regardless of the country value:


SELECT * FROM Customers
WHERE Country = 'Spain' AND CustomerName LIKE 'G%' OR CustomerName LIKE 'R%'



