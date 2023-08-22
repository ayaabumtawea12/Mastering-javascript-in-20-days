![Screenshot (999)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/27647193-9c7a-43b9-a270-c85cfb5f5235)##  conversion corner

## implicit coercion:-
Implicit coercion: Implicit coercion refers to JavaScript attempting to coerce an unexpected value type to the expected type. So we can pass a string where it expects a number, an object where it expects a string, etc, and it will try to convert it to the right type.

     let x;
     x = 8;
     x = x + "";
     // X will convert into string
     console.log(x, typeof x);
     x = x - 2;
     console.log(x, typeof x);
     
Output:

8 string
6 'number'
============================
![Screenshot (997)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/52a1465a-d221-4fa5-8697-188f62c6de75)
![Screenshot (999)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/659a9647-8a2a-49a7-b53d-63a0ea999617)
=========================
 ## Equality:

==  vs ===
![Screenshot (1001)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/2dfb13a2-db61-45c2-ae1a-a04362c890c1)

![Screenshot (1003)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/1b6f7f3f-d38f-4c15-9efc-3ae3947aa514)

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d8c036d4-2fc1-4c1a-a580-123cdcba0388)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/843d8fda-a23f-4640-9c5f-29f2d57c40ad)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/ec6a0834-d5fd-4569-83c8-c6d99dc3a365)
===============
**note
"12" == 12 ==>true
[] == [] ==> false
[] == ![] ==>true
false == [] ==> true
================
![Screenshot (1009)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/c80c0c85-1561-4baf-b5dd-92ea86fdc0d6)
==========

let a = 1;
let b = 1;
console.log(a == b); // true
let c = 10;
let d = "10";
console.log(c == d); // true
 
 
const name1 = {
    first_name: "sarah",
};
 
const name2 = {
    first_name: "sarah",
};
 
console.log(name1 == name2); // false

Output
true
true
false
===================
let a = 1;
let b = 1;
 
console.log(a === b); // true
let c = 10;
let d = "10";
 
console.log(c === d); // false
 
const name1 = {
    first_name: "sarah",
};
 
const name2 = {
    first_name: "sarah",
};
 
console.log(name1 === name2); // false

====================
## TypeScript 

















