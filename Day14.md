## Scope
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
================================
**Strict Mode
In "Strict Mode", undeclared variables are not automatically global.

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










