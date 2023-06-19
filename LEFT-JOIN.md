## LEFT JOIN 
Bierze wszystko z tabelki 1 plus część wspólną z tabelki 2

```
SELECT column_name(s)
FROM table1
LEFT JOIN table2
ON table1.column_name = table2.column_name;
```
```
SELECT Customers.CustomerName, Orders.OrderID
FROM Customers
LEFT JOIN Orders 
ON Customers.CustomerID = Orders.CustomerID
ORDER BY Customers.CustomerName;
```
- CustomersName wszystko i dane z innej tabelki które są wspólne, a tych których nie ma zastępuje słowem null