![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/5225f3f0-3090-4ff5-bf38-853933e2160c)## Database
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
====================================================
## At the INTERSECT

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/0e1644e3-8a9f-4fa2-bb12-fafabf4dd660)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/1391d4b3-2643-441e-8b2f-bb862f13ca20)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/4c65178a-5593-4fde-9b85-b9bbeffbc05f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/f926930e-bf72-4151-9286-ead3c2cd0a5f)

=========================================================
## EXCEPT
((SAME FIELD ))
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/aa63b103-1a5a-4526-a206-6e27e60f48da)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/afaac9f3-e56e-462e-94f6-14395d803981)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/0f2ee198-4a88-42f6-92b7-65208691d9dc)
=========================================================
## Subqueries
## subquerying with semi joins and anti joins
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/fa08805c-0c8a-43f0-86cf-ea5df5772bbd)

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e81d0f59-faa3-42f7-b148-4acfb790ee5e)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/75330865-e122-42ef-bd85-809504bba7b4)4![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/473b5fc4-7050-49e1-9f97-2f21062c79c0)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7b1a0c3d-ec1c-4c45-8c3c-835dc8dc0f06)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/79b99922-6771-4816-969b-5cf059da7361)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/a392ebbc-afbe-4a0c-bc5a-cd74530ece59)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c2975487-b422-43dd-8073-7edcbe6d496e)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/0bc375be-b038-4b07-8dec-a972b09a9e4e)
==================================================================
## Subqueries inside WHERE and SELECT
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3e342097-f5d4-4efa-8f27-ef0ce991bcc7)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/54958573-483b-4395-ae15-e7251e452503)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/70714473-5492-400a-b55c-c695fdea030c)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/aae0ab3f-304c-45c3-afbb-c978bdbb177e)

====================================================================
## Subqueries inside FROM
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/09541d08-72ff-4596-893f-f26bcb7e3867)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/05006d46-faf0-4cef-b546-eebaf30f4b01)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e683b65c-d09a-4090-8565-ecdd3bc15107)

======================================================================
## We'll take the CASE
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b2ff1630-6847-402a-b8e6-a7663c9fc32c)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/a7e0774b-fe47-4941-9a25-fd1df23a9b7c)

## In CASE things get more complex
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7a29e44f-ac38-4b01-8ea5-96bccedab3e2)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/9a0a05b8-a3f2-4e30-8577-3c8c4423a173)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/faf3a1ea-48fb-4e0a-be82-0161d91670ea)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/bb0dd131-faeb-4b05-b38d-3587c0ae7a2f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d126dd8a-a4b7-45d3-9089-33c50604e133)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c4914ece-4568-4219-a563-73d47c032a7e)

## CASE WHEN with aggregate functions
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c219fba0-33f7-4e72-a076-c830340bb74d)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/f1d1de7d-8302-4a91-afb2-4698bb257918)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/5d6a8d99-5a72-431d-bcea-e9d2a4009a82)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e2fe92b3-9a5a-4a44-9a66-a5646b85875e)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/8898c5bc-9dba-44c1-bbbe-8f84721f5a1f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d4bb6cd3-0742-4334-8d7f-198a98349149)
=============================================
## Short and Simple Subqueries

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/45f848d3-c0aa-4e67-90bb-fe8e2eb127d7)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/88e45675-f8dc-4a32-b8a4-eb50a1ce72d6)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/31e43d98-5e7b-47e8-b1f6-1a85fd106cef)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/847e30e2-dbe4-4d82-a934-bd7c11bcc20d)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/6e798b81-cd27-4f99-a6ef-59db1e5dd204)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/1fc49212-0365-40f9-a81b-7087af7ce037)
==============================================
## Subqueries in FROM
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/70a95808-8611-4efc-a6e6-2eab21828d38)


======================================
## Subqueries in SELECT
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b3b8d6fd-d77b-49f9-bdda-d6a747d77fb0)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/6dc15d3b-b873-40c9-ac0f-7db4567f5378)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/dcd03bb5-43d2-4c83-9420-9336f64f2193)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c9f56470-0a09-44e3-b723-56d562e69675)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3e350362-0979-450d-ac84-7577c0b597e1)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/eeebc2af-15f9-4791-b3f3-d3d6d7c5a9c0)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c280350d-a055-4e9b-857b-ca5fa214a218)
b![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/bb4bec11-f72c-4b62-8dba-b481b7d3a0f7)

=======================================
## Correlated subqueries:
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d419ca25-8a57-4abf-b542-116ce1d6ec5a)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/34fa6968-869d-4b7d-bf1f-7b002ec35b4c)


==========================
## Nested subqueries
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/e90b247b-5723-432f-a6eb-7d19e0a73113)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3b4152e2-afaf-419e-a1e8-5b4a618c1de9)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/1bfc677f-f0b4-49f1-9f1d-d688befcfa80)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/30c6c84c-616a-4182-9af1-a42c2c83340f)
============================================
## Common Table Expressions
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/2b525c92-9db6-4792-abbd-9e9c9b7e8edf)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/cb64a43a-61eb-4581-be5d-4bcf958df5bd)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7bf7cbf8-9a55-4c97-b4f5-ae0f3bef93e4)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/900b40f4-cf18-4175-a06b-34389f844c5b)
=============================================
## Deciding on techniques to use
=========================
## over (window)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/2125a720-922c-4dae-a02d-b293c533a8ae)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/bcf7e62e-e99b-4a17-b591-a59684e0ef3b)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3a92b74f-a869-4cb0-9daa-eb839b3f5510)
==================
##  OVER with a PARTITION
===========================
## Sliding windows
=========================
## Bringing it all together
==========================
## Pivoting
Pivoting(تحريك) rows to columns

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d83cd1ea-b192-4856-8a5f-24d498a0b866)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/5fd5c6d2-f327-4b29-b9a7-cac6f846fe45)
====================
## Crosstab queries using PIVOT in SQL Server

CREATE EXTENSION IF NOTEXISTS tablefunc;
Enter CROSS TAB 

==========================
## ROLLUP and CUBE
ROLLUP in SQL is an extension of the GROUP BY clause, this SQL ROLLUP option allows the user to include extra rows that represent the subtotals, which are usually referred to as super-aggregate rows, along with a grand total row.
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/1c7f10b8-0b06-4d90-a2e1-6772d5cb2eb8)
========================
## A survey of useful functions
==============

## Database
-- Get the column name and data type
SELECT
 	column_name, 
    data_type
-- From the system database information schema
FROM INFORMATION_SCHEMA.COLUMNS 
-- For the customer table
WHERE table_name ='customer';
=================
## Date and time data types
Interval 
====
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/deba2282-3c0b-4cae-8dc1-100d444ced94)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/02557133-bf36-44ce-b616-63157031662f)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/3a3ddb64-9c29-4237-a7a5-a71b00c7a183)

====================
-- Select the title and special features column 
SELECT 
  title, 
  special_features 
FROM film
-- Use the array index of the special_features column
WHERE special_features[2] = 'Deleted Scenes';
هاد الكود بيرع العنوان والبيشال لما يكون الاندكس التاني .......

======================
Searching an ARRAY with ANY
SELECT 
  title, 
  special_features 
FROM film 
-- Modify the query to use the ANY function 
WHERE 'Trailers' = ANY (special_features);

As we saw in the video, PostgreSQL also provides the ability to filter results by searching for values in an ARRAY. The ANY function allows you to search for a value in any index position of an ARRAY. Here's an example.
==============================
Searching an ARRAY with @>
The contains operator @> operator is alternative syntax to the ANY function and matches data in an ARRAY using the following syntax.

WHERE array_name @> ARRAY['search text'] :: type[]
SELECT 
  title, 
  special_features 
FROM film 
-- Filter where special_features contains 'Deleted Scenes'
WHERE special_features  @> ARRAY['Deleted Scenes'];
============================





