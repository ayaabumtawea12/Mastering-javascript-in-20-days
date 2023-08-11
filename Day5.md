conditionals:-
if(4>5){
console.log("yes");
}else if(4>2){
console.log("hi");
}else{
console.log("no");
}
======================
if(1){
    console.log("4");
}===>4

if(0){
    console.log("4");
}//undefined
============================
Exercise:
let fistname="aya";
let lastname="abu mtawea";

if(firstname.length>lastname.length)
{
console.log(firstname+"is longer than"+lastname);
}else{
console.log(lastname+"is longer than"+ firstname);
}
==============================================
function arr(array){
if(array.length === 0){
return true
} else{
return false;
}

arr([1,2,3])==>false
===============================================
if([])
{
console.log("true");
}=====>true

====================
if("")
{
console.log("true");
}else{
console.log("false");
}=====>false
=========================
if(null)
{
console.log("true");
}else{
console.log("false");
}=====>false
*****
if(undefined)
{
console.log("true");
}else{
console.log("false");
}=====>false
============================
if("false")
{
console.log("true");
}else{
console.log("false");
}=====>true
================================**********************************===================================
Logical:= and=> && **   or=>|| 
Ternary operator:-   condition ? valueiftrue : valueiffalse  =>for write quick condition 
if(x==3)                               
{                        equevalent       x==3 ?"yes":"no";
console.log("yes");
}else{
console.log("no");
}
}
=================================================================================
Loop:
let number=[1,2,3];
for(let x=0 ;x<number.length; x++)
{
console.log(number[x]);
}

for(let n of number){
console.log(n) ==>1 2 3
}
======================================================================================
for(let n of "aya"){
console.log(n) ==>a y a
}
================================================================
Map & Filter:-
Map:=> calls a function on each item in an array to create a new array
arrow function useful for this.

const numbers = [1, 2, 3, 4];
const doubled = numbers.map(item => item * 2);

filter: =>method takes each element in an array and it applies a conditional statement against it

const numbers = [1, 2, 3, 4];
const evens = numbers.filter(item => item % 2 === 0);
console.log(evens); // [2, 4]
============================================================
**Spread: we use it to put all item  from one array inside another array
let x=[1,2,3]
let y=[4,5,6]

let w=[...x,...y]; equivelent  let z=x.concat(y);
===========================================================
Array are like object?//true
===========================================================
While loop:-
let x=[];
while(x.length<5){
x.push(Math.random());
}
================================









===========================================================
Q1:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-multiple-conditional-ternary-operators
function checkSign(num) {
return num > 0 ? "positive" : num < 0 ? "negative" : "zero";
}

checkSign(10);
====================================
Q2:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-map-method-to-extract-data-from-an-array
// The global variable
const watchList = [
  {
  ........
  }
];

// Only change code below this line
let ratings=watchList.map(movie=>{
  let refinedMovieData={};
  refinedMovieData["title"]=movie["Title"];
  refinedMovieData["rating"]=movie["imdbRating"]
  return refinedMovieData;
})
 

// Only change code above this line

console.log(JSON.stringify(ratings));
================================================================
Q3:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-filter-method-to-extract-data-from-an-array
=======
Q4:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/golf-code
const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

function golfScore(par, strokes) {
  // Only change code below this line
if(strokes === 1){
return "Hole-in-one!";
} else if(strokes <= par-2)
{
return "Eagle";
} else if(strokes <= par-1)
{
return "Birdie";
} else if(strokes === par)
{
return "Par";
}
else if(strokes === par+1)
{
return "Bogey";
}
else if(strokes === par+2)
{
return "Double Bogey";
}
else if(strokes >= par+3)
{
return "Go Home!";
}

  return "Change Me";
  // Only change code above this line
}

golfScore(5, 4);
==================











