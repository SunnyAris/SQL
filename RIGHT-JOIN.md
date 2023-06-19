## Right Join
Bierze coś z tabelki 2 plus część wspólną z tabelki 1

```
SELECT column_name(s)
FROM table1
RIGHT JOIN table2
ON table1.column_name = table2.column_name;
```
```
SELECT Orders.OrderID, Employees.LastName, Employees.FirstName
FROM Orders
RIGHT JOIN Employees 
ON Orders.EmployeeID = Employees.EmployeeID
ORDER BY Orders.OrderID;
```

Bierze wszystko z tabelki Employees i dopasowuje do orders id jeśli nie ma jakiegoś numeru orderu wpisuje null 

```
SELECT *
FROM Orders
RIGHT JOIN Customers
ON Orders.CustomerID=Customers.CustomerID;
```

wszystko z tabelki customers i wspólne z tabelki orders 