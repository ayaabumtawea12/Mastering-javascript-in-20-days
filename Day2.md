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




