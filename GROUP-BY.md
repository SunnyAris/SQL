## GROUP BY 
# grupuje wiersze o tej samej wartości na przykład: AVG (), MAX(), COUNT(), MIN()


```
SELECT ProductID, ProductName, MAX(SupplierID) - MIN(CategoryID) 
As Odejmowanie ,MAX(SupplierID), MIN(CategoryID) FROM Products 
Group by ProductID;
```


```
SELECT COUNT(CustomerID),Country
FROM Customers 
GROUP BY Country;
```

- przelicza ilu jest customerów z danego kraju 


```
SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country
ORDER BY COUNT(CustomerID) DESC;

Count (CustomersID)           Country 
13                           USA
11                           France
11                           Germany
```
- Podlicza ilu jest customerów z danego kraju malejąco


```
SELECT Shippers.ShipperName, 
COUNT(Orders.OrderID) 
AS NumberOfOrders 
FROM Orders
LEFT JOIN Shippers 
ON Orders.ShipperID = Shippers.ShipperID
GROUP BY ShipperName;
```

- podlicza ile zamówień było zrobionych przez danego shippername zmieniając nazwę na numbersoforders


```
SELECT Customers.CustomerName, 
COUNT(Orders.OrderID)
AS NumberOfOrders 
FROM Orders
LEFT JOIN Customers 
ON Orders.CustomerID = Customers.CustomerID
GROUP BY CustomerName;
```