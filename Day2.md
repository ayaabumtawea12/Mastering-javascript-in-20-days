****EXPRESSION
LIKE variables, operators.
"aya abumtawea".includes("abumtawea")=>true
Operators:
3+4 => 7

***VARIABLES:
we create variable in js using
A)(let)
EX: let x=5;//we create variable x.
===========================================================================
1)Declaring a variable:-
let name;//declare var name
name; //undefined because you should assign this value

2)Assigning a variable:-
let name;
name="aya";asign variable name
name; =>"aya"
let x=null;
x; =>null;

Declaring and Assigning variable at once
let name="aya";
name =>variable || 'aya'=>value

B)constant
const x=3;//Declaring and Assigning variable 
===============================================================================
*****Statement vs Expression
let x=3;
 let,x,3  are expressions
 But if we take all of them together let x=3 then we have a statement
Statement( function Statement,loop Statement , if statement)
if( true ) {
    let status = "you should know I mean it"; 
    console.log(status)
}//if statement
==================================================================================
*****Arrays:
An array is a special variable, which can hold more than one value.
let x=['aya','bana','sara']//array of string
x.length ==>3
x.indexOf('aya'); ==>0 //aya index of 0
x[1]; ==>'bana'

*we can modify any value in array
x[1]="haya";
x; =>['aya','haya','sara'];

**delete last item in array
let y=x.pop();
x;==> ['aya','haya']
y;=>sara

***ADD item at the end of the array
x.push("zain");
x;=>['aya','bana','sara','zain']

##note
"aya"==["aya"];==>true
"aya"===["aya"];==>false

'aya'[0]=>'a'
['aya'][0]==>'aya'

-Array can be empty or contain single item 
EX:- let x=[] //empty array || let x=['aya'] //single item 

-Array can hold any type of item or mix
EX:- let arr=['aya',2,'a',false];

*****Array methods:-
let arr=['a','b','d','c'];
1-Sort 
arr.sort() ==>['a','b,'c','d'];

2-join
arr.join('&');==>'a & b & c & d'

3-concat
arr.concat(['e','s','k']);==>['a','b','d','c','e','s','k'];

--note
arr.push(['f','h','l']);
arr;==>['a','b','d','c',['f','h','l']]///nested array

==***Mutating Data
1-let x=['a','b','d'];
x[1]='c'
x==>['a','c','d'] ///mutable data Which data cne be edited

2-let str="abc";
str[0]='m';
str;==>'abc'////imutable data Which data stays the same as string and other primitives data.

***************
let y=[1,2,3,4,5]
y.concat([6,7,8]);
y;==>[1,2,3,4,5,6,7,8]

--immutable variable and mutable value
const x=[4,6];
let sum =x[0]+x[1];
sum;==>10

x[0]=6;

let sum =x[0]+x[1];
sum;==>12

***array is mutable data can change and edited in values***
***immutable data is the best***


***VARIABLES AND ARRAY***
let arr1=[1,2,3];
arr1;==>[1,2,3]

let arr2=arr1;
arr1[0]=5;
arr1;==>[5,2,3]
arr2;==>[5,2,3]

note:arr2 change also (arr2 ref to arr1 when arr1 change arr2 always equal arr1)


===========================================
*****OBJECT IN JS 
let x={key:value};
let obj={name:"aya",age:22};
obj.name;==>'aya'//way to access value in object
obj.name.sartWith('a')==>true
obj.name='haya';//change value
obj;==>{name:"haya",age:22};
obj.major="Eng";//add probarity to object
obj;//print object ==>{name:"aya",age:22,major:'Eng'};////object is mutible because it can be changed.
====================================================================================================================
QUESTION #1
Consider the following JavaScript code:

let a = 0;
let b = "0";
let c = false;
let d = "false";

console.log(a == b);===>result is true because == compare value just. not with data type
console.log(b === c);===>result is false because === compare value and data type
console.log(!!d);===>result is false because (!d) Negation of d=>true and  (!!d) false.
 
What will be the output of each console.log statement? You MUST explain WHY.
===========================================================================================================================
QUESTION #2:
Consider the following JavaScript expression:

console.log(4 + 5 * "7");
What will be the output of this expression? You MUST explain the steps of evaluation taken by JS.
the result is 39 (5*'7'=35)...35+4=39
==============================================================================================================================
QUESTION #3:
Evaluate the following expression:

let result = 5 + 2 * 3 - 1;
What will be the output of this expression? You MUST explain the steps of evaluation taken by JS.
result is 10(2*3=6 then 6-1=5 then 5+5=10) //priority to mul
===============================================================================================================================
QUESTION #4:
Consider the following code:

let x = 10;
let y = '10';
1-console.log(x == y);
2-console.log(x === y);
What will be the output of each console.log statement? You MUST explain WHY.
1-result is true because 10=='10' equal in value
2-result is false because 10==='10' equal in value but not equal in data type
======================================================================================================================================
QUESTION #5:
Given the code below:

let num = "15";
let isPositive = true;
let result = (num > 10 && isPositive) || num < 0;
console.log(result);
What is the value of result? You MUST explain the steps of evaluation taken by JS
num > 10==>true ,isPositive==>true then true&&true==>true then  num <0 ==> false so true || false ==>true so the result is true
=====================================================================================================================================


