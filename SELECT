SELECT - do wyszukania czegoś


SELECT * FROM Customers 
wyselektuj *(wszystkie) z folderu nazwa folderu
SELECT CustomersName FROM Customers
wyselektuj jedną kolumnę z folderu


SELECT CustomersName,ContactName FROM Customers
wyselektuj dwie lub więcej dzięki , kolumnę z folderu


SELECT DISTINCT Country FROM Customers
wyselektój kraje bez powtórek z folderu Customers 


SELECT CustomerName AS Imię, City AS Miasto From Customers 
zmienić nazwę kolumny np z Name na Imię


SELECT CustomerName FROM Customers WHERE CustomerID=1
wyselektuj z kolumny customer name z folderu gdzie id jest równe 1


SELECT * FROM Customers WHERE CustomerID=1
wyselektuj z wszystkich kolumn custumer id1


SELECT * FROM Customers WHERE Address='Obere Str. 57'
wyselektuj z wszystkich kolumn z folderu customers dany adres lub inne dane


SELECT * FROM Customers WHERE Address='Obere Str. 57' AND City='Berlin'
wyselektuj adres i miasto


SELECT * FROM Customers WHERE Address='Obere Str. 57' OR 'Berlin'
adres lub miasto 


SELECT * FROM Customers WHERE Address='Obere Str. 57'AND 'Berlin'
adres i miasto 


SELECT CustomerID, City AS Miasto FROM Customers WHERE City='London'

SELECT * FROM Customers
WHERE City IN ('Paris','London');


SELECT * FROM ordering WHERE customer_name LIKE 'Paul%'



SELECT * FROM Customers WHERE City LIKE 'B%'
wyselektuj miasta na B


SELECT CustomerName AS Nazwa FROM Customers WHERE CustomerName LIKE 'B%'

SELECT DISTINCT(City) * FROM Customers WHERE City LIKE 'B%'
pokazuje miasta na b bez duplikatów


SELECT * FROM Customers WHERE City LIKE '%B'
kończy się na b



SELECT * FROM Customers WHERE Address LIKE'%1'
adres kończy się na 1 

 SELECT DISTINCT(customer_name) FROM ordering WHERE customer_name LIKE '%paul%' HAVING  10 
imię paul ograniczenie do 10

SELECT COUNT(customersName) FROM Customers
 podlicza ile pozycji jest w kolumnie 


SELECT COUNT(customersName) AS LiczbaOsob FROM Customers
podlicza i zmienia nazwę


SELECT SUM(Price) From Products 
podlicza sumę liczb z danej kolumny


SELECT MAX(Price) From Products 
max liczba z kolumny


SELECT MIN(Price) From Products 
minimalna suma


SELECT ProductName, MIN(Price) From Products 
nazwa i min 


SELECT AVG(Price) FROM Products 
średnia np cena produktu AVG


SELECT ProductName, Price FROM Products 
wyselektuj nazwę, cenę 


SELECT ProductName, Price*100 FROM Products 
wyselektuj nazwę i cenę i pomnóż ją przez 100


SELECT ProductName, Price*100 AS Cena FROM Products
i zmień nazwę 


SELECT ProductName, Price/100 FROM Products
podziel na 100


SELECT ProductName, Price+100 FROM Products

SELECT * FROM Products WHERE Price>50
wyświetla cenę większą niż 50 z folderu 


SELECT * FROM Products WHERE Price>=50
większa równa


SELECT * FROM Products WHERE Prce!=18  
!= pokazuje wyniki poza wpisaną liczbą


SELECT * FROM Products WHERE Price!=18 AND Price!=19
cena poza 18 i 19 


SELECT * From Products WHERE Price BETWEN 50 AND 100 
cena pomiędzy 50 a 100


SELECT * From Products WHERE Price NOT BETWEEN 50 AND 100
cena nie jest pomiędzy 50 a 100





SELECT * FROM Orders WHERE CustomerID = 10 AND ShipperID >2



SELECT * FROM Customers WHERE CustomerID >10 AND Country='Mexico'


SELECT * FROM Customers WHERE CustomerID >10 OR CustomerID =7  



SELECT * FROM Orders WHERE CustomerID < 10 AND ShipperID >2
dane z 2 różnych kolumn w folderze 



SELECT Tytuł , Tresc FROM Ogloszenia WHERE Kategoria =1 AND podkategoria = 13 


AND - używamy gdy są to dane z dwóch różnych kolumn 

OR - gdy używamy danych z tej samej kolumny 
