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
 

🎆 ## Lexical scope 
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
✨lexical   Dynamic scope:

Dynamic Scope
In dynamic scoping, you search in the local function first, then you search in the function that called the local function, then you search in the function that called that function, and so on, up the call-stack.
## 
==



![Screenshot (1015)](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/614f221a-702d-48fe-96fc-63b301aba60d)
=================================
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













