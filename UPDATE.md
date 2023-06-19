## UPDATE
```
UPDATE Customers 
SET ContactName = 'Jan Kowalski' 
WHERE CustomerID = 3;  
```

- zmiana nazwy w kolumnie przypisanej id3 np zmiana imienia 

```
UPDATE Customers 
SET ContactName='Paweł', City='Kraków' 
WHERE CustomerID=3;
``` 

```
UPDATE Customers 
SET CustomerName = '', ContactName = '', Address = '', City = '', PostalCode = ''
WHERE Country = 'France';
```

- usuwa dane nie usuwając wiersza i zostawia tylko nazwę państwa

```
UPDATE Customers 
SET Address = '' 
WHERE CustomerID = 3;
```

- usuwa sam adres z wiersza dla id3

```
UPDATE Customers 
SET Country ='' 
WHERE CustomerID >= 80;
```

- usuwa kraj z wierszy wszystkich powyżej id80