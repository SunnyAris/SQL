UNION 
The UNION operator selects only distinct values by default. To allow duplicate values, use UNION ALL



SELECT column_name(s) FROM table1
UNION ALL
SELECT column_name(s) FROM table2;



SELECT City FROM Customers
UNION
SELECT City FROM Suppliers
ORDER BY City

