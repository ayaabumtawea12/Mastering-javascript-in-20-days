## Scope
-Nested
-Hoisting
-clousure
-Module

Scope determines the accessibility (visibility) of variables.
JavaScript has 3 types of scope:

Block scope
Function scope
Global scope

{
  let x = 2;
}
// x can NOT be used here
=====

{
  var x = 2;
}
// x CAN be used here
 


## Lexical scope 
is the ability for a function scope to access variables from the parent scope. We call the child function to be lexically bound by that of the parent function.
================================
✨Strict Mode
In "Strict Mode", undeclared variables are not automatically global.
The purpose of "use strict" is to indicate that the code should be executed in "strict mode".
With strict mode, you can not, for example, use undeclared variables.

'use strict';

x = 9; // ReferenceError: x is not defined    // This will cause an error because x is not declared
======
function strict_function() {
  'use strict';

  x = 'I am a strict function';

  console.log(x);
}

strict_function(); // ReferenceError: x is not defined

=====================
✨Nested Scope:-
A nested function is a function inside another function
We can create the nested function in the same way we create the normal JavaScript function, But inside another function

function addNum(a,b)
{
 
  //nested function
  function logToConsole(message)
  {
    console.log(message);
  }
 
  let result=a+b;
 
  //invoking the nested function
  logToConsole("result is "+result)
}
 
addNum(1,2)
 
***output ***
result is 3 



===============================
## Scope & Function Expressions 

The Javascript Function Expression is used to define a function inside any expression.
The Function Expression allows us to create an anonymous function that doesn’t have any function name which is the main difference between Function Expression and Function Declaration

function callAdd(x, y) {
    let z = x + y;
    return z;
}
console.log("Addition : " + callAdd(7, 4));

output: Addition : 11
========================
expression function :
The Javascript Function Expression is used to define a function inside any expression
et calSub = function (x, y) {
    let z = x - y;
    return z;
}
 
console.log("Subtraction : " + calSub(7, 4));
Output: 

Subtraction : 3

=======
let x=function(){console.log("aya")
x;//referanceerror
x();==>aya
============================
👀Arrow function
const materials = ['Hydrogen', 'Helium', 'Lithium', 'Beryllium'];

console.log(materials.map((material) => material.length));
// Expected output: Array [8, 6, 7, 9]
===================================================================
✨lexical  vs Dynamic scope:

## lexical scope:-
(Static Scoping)
s the ability for a function scope to access variables from the parent scope. We call the child function to be lexically bound by that of the parent function. The diagram below outlines the supposed hierarchy that the lexical scope maintains in JavaScript.

var a = 10
var func = function (){
var b = 20;
    console.log("a and b is accessible (outer):", a, b);
    var innerFunc= function (){
        var c = 30;
        console.log("a and b and c is accessible (inner):", a, b, c);
    }
    innerFunc();
    return;
}
func();
console.log("only a is accessible (global):", a);


![Screenshot (1018)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/1f1ff149-5668-4834-b15b-43a78c42a635)

## Dynamic Scope
In dynamic scoping, you search in the local function first, then you search in the function that called the local function, then you search in the function that called that function, and so on, up the call-stack.

let x=10;

function foo(){
console.log(x)
}

function print(){
let x=20;
foo();
}

print();


![Screenshot (1015)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/614f221a-702d-48fe-96fc-63b301aba60d)
========================================================
## Function Scope
JavaScript has function scope: Each function creates a new scope.

Variables defined inside a function are not accessible (visible) from outside the function.

Variables declared with var, let and const are quite similar when declared inside a function.

Thfunction myFunction() {
  var carName = "Volvo";   // Function Scope
}
===================================

## IIFE (Immediately Invoked Function Expression)🎇

A JavaScript immediately invoked function expression is a function defined as an expression and executed immediately after creation.
Ex:
(function(a,b){
        return a + b;
})(10,20);
========================================
## Block Scoping
-var:
Variables declared with the var keyword can NOT have block scope.

Variables declared inside a { } block can be accessed from outside the block.

-let and const.
Variables declared inside a { } block cannot be accessed from outside the block.

{
  let x = 2;
}
// x can NOT be used here
===================================

let x=3;
x= 4 //allow

const x=2;
x=5;type errr

varx=3;
x=4;allow

const x=[1,3]
x[1]=8;//allow

=======================================
## Hoisting:👀

-In JavaScript, a variable can be declared after it has been used.

-In other words; a variable can be used before it has been declared.

var x; // Declare x
x = 5; // Assign 5 to x

Using a let variable before it is declared will result in a ReferenceError.

carName = "Volvo"; //This will result in a ReferenceError:
let carName; 

-Using a const variable before it is declared, is a syntax error, so the code will simply not run.
carName = "Volvo";
const carName;


====================================================

function fun(){
        console.log(name);
        let name = 'Mukul Latiyan';
    }
    fun();//ReferenceError
    
================================

*****Function is hoisted:👀
fun(); // Calling before declaration
     
    function fun(){ // Declaring
        console.log("Function is hoisted");
  }
================================

## note:-👀

 if a function is used as an expression and we try to access it before the assignment an error will occur as only declarations are hoisted.
 fun() // Calling the expression
 
let fun = () =>{ // Declaring
    let name = 'Mukul Latiyan';
    console.log(name);
}

================================












===================================

## QUESTION #1
Given the following promisesArray, convert the array into an object using the convertToObj function.

You should apply typescript types to every promise, the input of convertToObj, and the output of convertToObj.

Build interfaces and types as needed.

https://github.com/orjwan-alrajaby/gsg-QA-Nablus-training-2023/blob/main/learning-sprint-1/week3%20-%20deep-javascript-foundations-v3/day%202/tasks.md

======================================

## QUESTION 2:
What will be the output of the following code snippet? Pick the right choice then justify your answer with an explanation.

function testScope1() {
  if (true) {
    var a = 1;
    let b = 2;
    const c = 3;
  }
  console.log(a);
  console.log(b);
  console.log(c);
}

testScope1();
Choices:

A) undefined, undefined, undefined
B) 1, undefined, ReferenceError
C) 1, ReferenceError, ReferenceError
D) 1, ReferenceError

🎈The answer is D
=====================================
## QUESTION #3:
What will be the output of the following code snippet? Pick the right choice then justify your answer with an explanation.

function testScope2() {
  console.log(a);
  console.log(b);
  console.log(c);
  if (true) {
    var a = 1;
    let b = 2;
    const c = 3;
  }
}

testScope2();
Choices:

A) undefined, ReferenceError
B) 1, undefined, ReferenceError
C)undefined, undefined, ReferenceError
D) 1, ReferenceError

🎈The answer is A
=========================================
## QUESTION #4:
What will be the output of the following code snippet? Pick the right choice then justify your answer with an explanation.

function testScope3() {
  var a = 36;
  let b = 100;
  const c = 45;

  console.log([a, b, c]);

  if (true) {
    var a = 1;
    let b = 2;
    const c = 3;

    console.log([a, b, c]);
  }

  console.log([a, b, c]);
}

testScope3();
choices:

A) [ 36, 100, 45 ] | [ 1, 2, 3 ] | [ 36, 2, 3 ]
B) [ 36, 100, 45 ] | [1, 2, 3 ] | [ 36, 100, 45 ]
C) [ 36, 100, 45 ] | [ 1, 2, 3 ] | [ 1,100, 45 ]
D) [ 36, 100, 45 ] | [ 1, 2, 3 ] | [ 1, 2, 3 ]

🎈The answer is B
============================================
## QUESTION #1
Create a function called arrowHOF that takes an arrow function as input and returns a new arrow function that enhances the behavior of the input function.

The enhanced function should accept additional arguments and execute the input function multiple times based on these arguments.

const exampleNormalFunc1 = (a, b, c) => {
  return a * (b + c);
}

const exampleNormalFunc2 = (x, y) => {
  return x * y;
}

const exampleNormalFunc3 = (string) => {
  return string + " " + string + " " + string + "!";
}


const arrowHOF = (normalFunc) => {
  // write your code here;
}

const hofNormalFunc1 = arrowHOF(exampleNormalFunc1);
const hofNormalFunc2 = arrowHOF(exampleNormalFunc2);
const hofNormalFunc3 = arrowHOF(exampleNormalFunc3);

console.log(hofNormalFunc1(3, 4, 5)(2)); // logs 60 twice
console.log(hofNormalFunc2(20, 35))(4); // logs 700 four times
console.log(hofNormalFunc3("Meow")()); // logs "Meow Meow Meow!" once

======================================================
## QUESTION #2
Build a function called preserveThis that takes a function as input and returns a new arrow function that behaves the same way as the input function but preserves the original this context when used as a method of an object.

// Example object
const obj = {
  name: 'John',
  greet: function (greeting) {
    console.log(`${greeting}, ${this.name}!`);
  }
};

const preserveThis = (func) => {
  // write your code here;
  
  return func;
}

// Wrap the greet function using preserveThis
const preservedGreet = preserveThis(obj.greet);

// Call the wrapped function as a method of the object
preservedGreet('Hello'); // Output: "Hello, John!"
===================================================
## QUESTION #3
Consider the 2 following examples and distinguish the different output in each one with them with a reasoning.

Example 1:

function outer1() {
  var x = 10;

  var inner1 = function() {
    console.log(x);
  };

  inner1();
}

outer1(); // Output: 10
Reasoning for example 1's output:
lexical scope child  take value from parent (outer1()) because havent value of x;

======================================================================

Example 2:

function outer2() {
  var x = 10;

  var inner2 = function() {
    var x = 20;
    console.log(x);
  };

  inner2();
}

outer2(); Output: 20

Reasoning for example 2's output:

lexical scope 
... child  uses the value of x not X in the parent...
============================================================================

## ADVANCED SCOPE:
QUESTION #1
Given the following code snippet and explain what's happening.

for (var i = 0; i < 5; i++) {
    setTimeout(function() {
      console.log("value of [i] is: ", i);
    }, 100);
}
The current output is: "value of [i] is: 5" five times.

The output should be:

"value of [i] is: ", 0 "value of [i] is: ", 1 "value of [i] is: ", 2 "value of [i] is: ", 3 "value of [i] is: ", 4

Without changing anything in the for loop's code itself, provide a solution to fix it.

for (var i = 0; i < 5; i++)(function(i) {
    setTimeout(function () {
     console.log("value of [i] is: ", i)
    }, 100);
})(i)
====================================================
## QUESTION #2
Given the following code snippet and explain what's happening.

for (let i = 0; i < 5; i++) {
   let array = [];
   array.push(i);
   console.log("Current array is: ", array)
}
The current output is:

"Current array is: [ 0 ]" "Current array is: [ 1 ]" "Current array is: [ 2 ]" "Current array is: [ 3 ]" "Current array is: [ 4 ]".

The output should be: "Current array is: [0, 1, 2, 3, 4]".

Provide a solution to fix it.

let array = [];
for (let i = 0; i < 5; i++) {
   array.push(i);
}
console.log("Current array is: ", array)
===============================================
## QUESTION #3
Given the following code snippet and explain what's happening.

let functions = [];

for (var i = 0; i < 5; i++) {
  functions.push(() => {
    console.log("Current value of i is:", i);
  });
}

functions.forEach((func) => func());
The current output is:

"Current value of i is: 5" "Current value of i is: 5" "Current value of i is: 5" "Current value of i is: 5" "Current value of i is: 5"

The output should be:

"Current value of i is: 0" "Current value of i is: 1" "Current value of i is: 2" "Current value of i is: 3" "Current value of i is: 4"

Provide a solution to fix it.

let functions = [];

for (var i = 0; i < 5; i++) {
  functions.push("Current value of i is:", i);
};

functions.forEach((func) => console.log(func));

========================================================




