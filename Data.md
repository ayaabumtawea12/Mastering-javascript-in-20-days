## Database
store and secure 
==================
 

## table

name lower 
no space maybe _
plural
row ==record
column ==fiels
===================
data type
string 
int
float

phone number must string or text.
===============================
## server 
store database 
and to make request 
===========================
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7e5153af-466b-401c-bf0b-fb3a891874c8)
![Screenshot (1026)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/24fef9c6-30b4-4d2d-8dcc-8f03b0a6bd2a)
![Screenshot (1025)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/ccca4aa4-1517-44b9-890f-cdfe97619355)
![Screenshot (1024)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/63820619-7ffd-4d51-b106-81fe6288c2df)
=========================
npm install cypress --save-dev
npx cypress open
tsc --init
npx -p typescript tsc --init
================================
## section 2
## Introducing queries

## keyword:
==========
SELECT column_name,c2
FROM
table_name;
============================
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/a1da4fdd-b81d-49d4-ac58-bb0bc91c79d7)
===========================

## Writing queries
## Aliasing (As)
to rename colums;
=================
SELECT  first_name As name ,last_name
FROM 
employees;
==================
## Distnict:-
without repeat row.
You've learned that the DISTINCT keyword can be used to return unique values in a field. 

SELECT DISTINCT  first_name ,last_name
FROM 
employees;
=======================
## VIEWS
virtual table
A view contains rows and columns, just like a real table. The fields in a view are fields from one or more real tables in the database.

A view is created with the CREATE VIEW statement. 

CREATE VIEW view_name AS
SELECT column1, column2, ...
FROM table_name
WHERE condition;

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/a5d4f9c7-1499-4f79-a173-f394f2f2b127)

=================
## SQL flavors
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d18c6a9b-d3f5-4926-a0a4-2379867924ed)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c4b5c9c7-1b05-4853-9825-e9d864c6369b)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/525d2fea-de9b-405e-810e-95a8951c6cb2)
==================
## Count:-
how records in field.
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/0c5bec18-429c-4ca8-84d6-792f50d74b97)

SELECT COUNT(FIRS_NAME)
FROM 
COURSES;

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/4d611f8f-2725-4774-bbb4-e00982861a52)

===============================
Query execution:
order of execution
Drag the SQL keywords into the order that they will be executed in (not the written order) from first (top) to last (bottom).
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8835a616-d38c-421e-b35e-29a5e053735a)

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/949adb7c-a859-438f-be93-447f64ca1ad9)












