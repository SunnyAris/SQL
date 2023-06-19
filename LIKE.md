## LIKE  
```
SELECT * 
FROM Customers 
WHERE ContactName 
LIKE '%n';
```
- nazwa kończy się na n

```
SELECT * 
FROM Customers 
WHERE ContactName 
LIKE 'p%n';
```
- nazwa zaczyna się na p kończy na n 


```
SELECT * 
FROM Customers 
WHERE ContactName 
LIKE '__s%';
```

- 3 literka to s daje się 2 podłogi przed s

```
SELECT * 
FROM Customers 
WHERE ContactName 
LIKE '_ar%';
```
- 2 literka a 3 literka r

```
SELECT * 
FROM Customers 
WHERE ContactName 
LIKE '_ar%s';
```
- na końcu s 

```
SELECT * 
FROM Customers 
WHERE ContactName 
LIKE '_____%';
```

- takie które mają przynajmniej 5 literek 