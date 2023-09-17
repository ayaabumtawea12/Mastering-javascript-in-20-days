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
## Query execution:
order of execution
Drag the SQL keywords into the order that they will be executed in (not the written order) from first (top) to last (bottom).
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8835a616-d38c-421e-b35e-29a5e053735a)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/949adb7c-a859-438f-be93-447f64ca1ad9)

====================
## sql styles:-
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/570e7266-7295-424c-97fc-6c1bc10b1299)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/ed98c7f4-40b8-4f16-b013-aee075718404)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/a9b7e174-8125-4c9f-a6d7-8d59baefa256)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/9a2fb4ac-658d-4b67-b3eb-68b8ffe24f17)

=====================
## Filtering Records
Filtering numbers
WHERE
EXAMPLE:
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8a698e95-c423-4d39-908f-c18509e942d5)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/a34e802a-a75d-4c16-9471-85dc006b2493)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3e8426f0-4a4f-4db9-ac0d-86e718c39164)
========
important
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/736b3eee-b3cd-40bc-8697-aa9edd8c9603)
===========
## Multiple criteria
OR,AND,BETWEEN
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c5ebdb56-6ce0-4fee-afa8-7239af50802c)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/cbadb4c8-4e75-492c-a0b3-4e46b80dee66)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/83514065-56a7-4825-811b-51a1604ead68)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d0394721-d576-4f3b-a799-f5cf48918b3a)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c095d4c0-54e8-436b-973d-fc2f5abe75c1)

============================
## Filtering text

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d4c6b7c1-94ac-41a7-a557-d534db6fa501)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/5fb5a7de-8d8b-402d-876f-68c26bf25a2f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/4c99d8fa-ddbd-4a78-9408-63f0de5ae459)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/5dab9b88-d05f-4311-9e35-f1099d1dd267)
=================================
## NULL values

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/18b2f11c-bc20-4b72-8d0a-48dbc0e8645f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/07aac74a-aef4-46e1-ae70-1d34c35dfdb7)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b939ad04-a1c0-4756-8362-6e3c0dee18af)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7d214540-cca9-47a1-aa93-b31688b9041e)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/add2950b-8c69-4582-b052-fe6dc4ea682c)
===============================
## Summarizing data
## AGGREGATE :

SUM,MAX,MIN,AVG,COUNT

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e51d85b2-0341-4cee-886d-85a68b237304)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e9761ca1-e77d-4218-9a45-e473b603e6ec)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/312f3e25-8748-4da3-b721-19bc874931a4)


=================================
## Summarizing subsets
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/9f4ff81e-537c-42ae-9203-7de6ddc5dbb4)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d7df50aa-64d4-419b-850e-3628743e5f07)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/0de10dc8-db09-4072-b84e-0a66eee03273)
====================================
## Aliasing and arithmetic
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/0beee63f-848f-46c5-8e06-0c6d7b082128)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b942e96c-ead4-429d-9880-6588fd997fb8)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/99415c38-d422-43b9-a562-0ea9ff382d9d)
========================================
## Sorting results:
ORDER BY==>ascending order by default. (A-Z).  alphabetically
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/2fa21726-d0c1-4178-addc-d7ced5d0a192)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/383e51e2-a72b-4b2e-9f17-4ba385e33f8e)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/34e1ede7-2cfc-42a6-91b5-6a804366dec3)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/112957c2-d4fd-4589-9341-5dbe7c40c087)
===========================================================
## Grouping data
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3455677c-6455-4939-a01e-23510d668f4d)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/eacbd3a1-e76c-445d-8860-35610d99a1c4)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/9fd78b7a-fcaa-413e-b261-7049a870ec80)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/80b275e8-c496-4cdd-9b8f-61b28e9d0387)
===================================================
## Filtering grouped data
HAVING ==== WHERE
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/4430ad5c-05d3-45fd-9ac9-be12bb019daf)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e8473dc7-3cf0-4e2b-95b1-2faa26c6a425)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3c8b4b0d-73ba-4e2e-bce7-9d26a316b0f5)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/5f104f08-0ee6-4727-9c59-38a0c7586d29)
=============================================
## The ins and outs of INNER JOIN

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/281e45f8-c265-415e-89c0-3bbe4ffdf198)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8611e1b7-361e-4377-a76d-de7ac6c74ee3)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/934bd971-38dc-4375-b34c-20713bbbe7cb)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/277c87b2-507c-48b0-8e11-a8a14520ac4f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/72f388f1-6df7-47f3-9810-bb4087f8c395)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b25aec48-322f-49ad-b175-f5fc3a4a371d)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7514cfe9-eeae-4e0f-bbfe-4f6299cb96c2)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7cacadc0-5cdf-4fa3-ab07-2de4150b2328)

===============================================
## Defining relationships
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/96910e11-bfbc-4e76-91dc-cbd5da9bf4f0)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/166f9481-8afe-4601-a9e6-1d7890e8361f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/683db396-76c8-4175-839d-e3c892bf95d1)

==================================
## Multiple joins
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/68c21337-2b1b-446e-a85b-7ae2cceb2833)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b6a8ae00-fc48-41bb-932c-1b419e9e12b4)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8bcc877b-9efe-4078-b6ac-8daf2861dc40)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/dcef1b2b-58a6-4003-ac29-af53e2d4ce39)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e4d54f72-a34b-478f-8f22-9f3e52ff9507)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b1f25dc7-c935-47ad-a52a-5c1ecec4dd1a)
=========================================
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/dbad6241-e92c-4dac-9f3f-b297b295eb0a)
================
## LEFT and RIGHT JOINs
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/92a1203c-461f-404b-b01d-978ce3bc5624)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/9a44a47e-234e-4d71-bdf0-97369437e96a)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d3204e77-20ff-4c3d-9efa-b0e68ec94435)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8b67fdab-0ea0-465f-bf94-6f97735ad1fd)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/aabc865b-fd17-4e78-823e-50a426834477)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8987f668-2173-41bc-8349-1b20ed2b8467)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/1179187a-8b24-4917-b4be-07232c7436c9)
===================
## Crossing into CROSS JOIN


========================
## Self joins
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/4e4e349d-9a43-4448-ab45-b5319d5eb3d3)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/9d7f604b-7650-470b-85f0-11c596c8048f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7778c886-1cbd-4643-b248-67171deb82bc)
===================================================
## Set theory for SQL Joins
****same field in two tables and same number of fieled ,same data type.
اﻷمر UNION فقط يوجد فرق واحد وهو أن اﻷمر UNION ALL لا يقم بحذف البيانات المكررة عكس اﻷمر UNION
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/4093fd65-07fb-4b9f-9a4b-6af8fb419a5f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d380edc6-9fed-4313-b046-db93818f9bd2)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/ed2cbdaa-afb8-4e55-a492-b6a1dae7ec31)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/bd439002-cba2-4173-80f2-7c5815954878)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8f611a1a-e147-42e8-9a86-6fbb0ebc4dc4)
















