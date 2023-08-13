call stack in js:-
used by JavaScript to keep track of multiple function calls. It is like a real stack in data structures where data can be pushed and popped and follows the Last In First Out (LIFO) principle.

function f1() {
    console.log('Hi by f1!');
}
 
function f2() {
    f1();
    console.log('Hi by f2!');
}
 
f2();
////"Hi by f1!"
"Hi by f2!"
=================================================
Repeating functionality:-
function mularray(let arr[]){
let out=[];
for(let i=0;i<arr.length;i++){
out.push(arr[i] * 2);
}
return out;
}

let myarr=[1,2,3];
let result=mularray(myarr);
============================================
Higher Orders Functions:-
are functions that perform operations on other functions.
A higher order function is a function that takes one or more functions as arguments, or returns a function as its result.

const numbers = [1, 2, 3, 4, 5];

function addOne(array) {
  for (let i = 0; i < array.length; i++) {
    console.log(array[i] + 1);
  }
}

addOne(numbers);
The function addOne() accepts an array, adds one to each number in the array, and displays it in the console. The original values remain unchanged in the array, but the function is doing something for each value.

==================================================
// Callback function, passed as a parameter in the higher order function
function callbackFunction(){
    console.log('I am  a callback function');
}

// higher order function
function higherOrderFunction(func){
    console.log('I am higher order function')
    func()
}

higherOrderFunction(callbackFunction);


=================================================
Q1:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-higher-order-functions-map-filter-or-reduce-to-solve-a-complex-problem















