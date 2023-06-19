## HAVING


```
SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country
HAVING COUNT(CustomerID) > 5;
```
- Grupuje listę customers z danego kraju gdzie customerów było więcej niż 5


```
SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country
HAVING COUNT(CustomerID) > 5
ORDER BY COUNT(CustomerID) DESC;
```

- Grupuję listę customers z danego kraju gdzie kustomerów było więcej niż 5 malejąco 


```
SELECT Employees.LastName, COUNT(Orders.OrderID)
AS NumberOfOrders
FROM Orders
INNER JOIN Employees 
ON Orders.EmployeeID = Employees.EmployeeID
GROUP BY LastName
HAVING COUNT(Orders.OrderID) > 10;
```
- Grupuję listę pracowników z większą liczbą zamówień niż 10
plus zmiana nazwy kolumny 


```
SELECT Employees.LastName, COUNT(Orders.OrderID) AS NumberOfOrders
FROM Orders
INNER JOIN Employees 
ON Orders.EmployeeID = Employees.EmployeeID
WHERE LastName = 'Davolio' 
OR LastName = 'Fuller'
GROUP BY LastName
HAVING COUNT(Orders.OrderID) > 25;
```
- to samo dodając konktetne nazwisko 

