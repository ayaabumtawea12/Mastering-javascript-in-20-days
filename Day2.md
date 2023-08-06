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


===========================================




