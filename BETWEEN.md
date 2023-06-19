## BETWEEN

```
SELECT * 
FROM Orders 
WHERE OrderDAte >= '1996-07-01' 
AND OrderDate <= '1996-07-10';
```

- wyszukuje daty pomiędzy 


```
SELECT * 
FROM Orders 
WHERE OrderDate 
BETWEEN '1996-07-01' AND'1996-07-10';
```

- to samo co wyżej tylko krócej zapisane 


```
SELECT * 
FROM Orders 
WHERE EmployeeID 
BETWEEN 1 AND 4;
```

- id pomiędzy 1 a 4 