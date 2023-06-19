## ORDER BY sortowanie
- sortuje w porządku rosnącym, malejący 
używany po gruped by



### The following SQL statement selects all customers from the "Customers" table, sorted ascending by the "Country" and descending by the "CustomerName" column:



ASC Rosnąco 

DSC majejąco 


```
SELECT * 
FROM Employees 
ORDER BY LastName
```

- sortowanie po nazwusku 

aby dobrze posortować gdy są dwie osoby o tym samym nazwisku dodajemy firstname

```
SELECT * 
FROM Employees 
ORDER BY LastName, FirstName;
```

```
SELECT * 
FROM Employees 
ORDER BY LastName DESC, FirstName DESC;
```

- jeśli chcemy aby i imię i nazwisko było posortowane malejąco dodajemy desc 2 razy


```
SELECT * 
FROM Customers
ORDER BY Country, CustomerName;

```

- posortuje państwa a jeśli będą powtórki dodatkowo przez customername


```
SELECT * 
FROM Customers
ORDER BY Country ASC, CustomerName DESC;
``` 

- kraj rosnąco customername malejąco