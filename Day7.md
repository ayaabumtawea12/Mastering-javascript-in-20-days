## call stack in js:-
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
## Repeating functionality:-
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
## Higher Orders Functions:-
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
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-higher-order-functions-map-filter-or-reduce-to-solve-a-complex-problem.
const squareList = arr => {
  // Only change code below this line
let sqnum=arr.filter(num=>{
  if(Number.isInteger(num) && num>0)
  {
    return num;
  }
}).map(num=> {return num*num})
  return sqnum;
  // Only change code above this line
};

const squaredIntegers = squareList([-3, 4.8, 5, 3, -3.2]);
console.log(squaredIntegers);
================================================================
Q2:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/apply-functional-programming-to-convert-strings-to-url-slugs
// Only change code below this line
var wisc="Winter Is Coming";

function urlSlug(title) {
return title
.slice()
.toLowerCase()
.split(" ")
.filter(word => {
  if(word != "")
  {
    return word;
  }
}).join("-")
}

// Only change code above this line
var tit=urlSlug(wisc);
console.log(tit)
=======================================
Q3:
https://github.com/orjwan-alrajaby/gsg-QA-Nablus-training-2023/blob/main/learning-sprint-1/week2%20-%20javaScript-the-hard-parts-v2/day%201/tasks.md
Question 1: Functions and Callbacks
Implement a JavaScript function called mapAsync that takes an array and a callback function. The function should map each element of the array to a new value using the callback function asynchronously.
The final result should be returned as a Promise.

const array = [1, 2, 3];

const asyncRes = await Promise.all(array.map(async (i) => {
	await sleep(10);
	return i;
}));

console.log(asyncRes);

================================
Question 2: Call Stack and Recursion
Write a JavaScript function called sumRange that calculates the sum of all integers in a given range. The function should use recursion to handle the calculation and demonstrate understanding of the call stack.

function sumRange(n)
{
    if (n <= 1)
        return n;
    return n + sumRange(n - 1);
}
  
let n = 5;
console.log(sumRange(n));
















