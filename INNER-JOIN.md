

## INNER JOIN łączy wspólne dane z innych folderów 

```
SELECT OrderID, EmployeeID, OrderDate 
FROM Orders; 
```
pokazują się dane dotyczące osoby 

```
SELECT column_name(s)
FROM table1
INNER JOIN table2
ON table1.column_name = table2.column_name;
```

```
SELECT Orders.OrderID, Employees.FirstName, Employees.LastName, Orders.OrderDate 
FROM Orders 
INNER JOIN Employees 
ON Orders.EmployeeID = Employees.EmployeeID 
```
miesza dane z dwóch tabel które są jakoś ze sobą powiązane będąc w zakładce orders pobieramy dane dotyczące osób z zakładki employees gdzie podane są dane na których nam zależy dodatkowo używając on aby połączyć to z id które jest wspólne dla tych odób w oby folderach  


```
SELECT Customers.CustomerName, Customers.City, Customers.Country, Suppliers.SupplierName 
FROM Customers
INNER JOIN Suppliers 
ON Customers.Country = Suppliers.Country 
```



```
SELECT Orders.OrderID, Employees.FirstName, Employees.LastName, Orders.OrderDate, Shippers.ShipperName, Shippers.Phone 
FROM Orders 
INNER JOIN Employees 
ON Orders.EmployeeID = Employees.EmployeeID 
INNER JOIN Shippers 
ON Orders.ShipperID = Shippers.ShipperID
```

do poprzednich informacji dodajemy dane z 3 tabeli dotyczące wysyłki i numeru telefonu z folderu shippers  


```
SELECT Orders.OrderID, Employees.FirstName, Employees.LastName, Orders.OrderDate, Shippers.ShipperName, Shippers.Phone,
Customers.CustomerName 
FROM Orders 
INNER JOIN Employees 
ON Orders.EmployeeID = Employees.EmployeeID 
INNER JOIN Shippers 
ON Orders.ShipperID = Shippers.ShipperID
INNER JOIN Customers 
ON Orders.CustomerID = Customers.CustomerID 
```

dodatkowo połączone z kolejnym folderem customers 

```
SELECT "Album"."Title", "Artist"."Name", "Track"."Composer"
FROM "Album"
INNER JOIN "Artist" 
ON "Album"."ArtistId"="Artist"."ArtistId"
INNER JOIN "Track" 
ON "Album"."AlbumId"="Track"."AlbumId"
```