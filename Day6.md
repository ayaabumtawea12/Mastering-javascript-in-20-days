Fetching data:
APIs provides a URL that point at data we care about.
fetch("url......") load data from API;
it take time to fetch data from network.....

A-Promises
can be in 3 possible states:
1-pending
2-fufilled
3-rejected

B-A wait 
lets us tell js to stop and wait for an async operation to finish.

let response=await fetch("...")
console.log(response);

let body= await response.json();//return data ;
fetch(" ").then((value)=>console.log(value));
===========================================================
Destructing data:-
Destructiong object & Array:
is a funcy way of declaring multible variable at once.

 const arr =[{name:"aya", age:22}]
 let {name,age}=arr[0];//create var name and age.//destruct object
 name==>aya
 ============================================================
 destruct array:
 const [one,ewo,three]=[1,2,3];
 console.log(one);//1
 console.log(three);//3

 let {title}=document;
================================
let [one, ...others]=[1,2,3,4];
one=>1
others=>[2,3,4]

note:****************************************
split()////return array
"Aya Abu Mtawea".split("");==>["Aya","Abu","Mtawea"];
let [first,second,thired]="Aya Abu Mtawea".split("");

first;=>"Aya"

***** "Aya Abu Mtawea".split("-");==>["Aya Abu Mtawea"];
***** "Aya-Abu-Mtawea".split("-")join(" "); ==>"Aya Abu Mtawea"
let [a,b]= "Aya Abu Mtawea".split("-");
["aya","abu mtawea"].join(" ");==>"aya abu mtawea"
["aya","abu mtawea"].reverse();==>["abu mtawea","aya"]
=========================================
FETCH:
function fetch(url){
let x=await fetch(url);
return x.json();
}
////////error this not allow in js

************
async function fetch(url){
let x=await fetch(url);
return x.json();
}//////this tell js to expect  to await async operations inside the function. 
 ///true 
 fetch("url");
==========================================================
async function fetch(url){
let response=await fetch(url);
let body= response.json();
let {message}=body;
return message;
}//////this tell js to expect  to await async operations inside the function. 
 ///true 
 await fetch("url");
===================================
***Modules:-
 module.js//file name
 
 let x="aya"
 export {x};

anothwr file 

import {x} from './module.js';
x;=>aya
 

================================
DEBUGGING:-
Errors can (will) happen, every time you write some new computer code.
all modern browsers have a built-in JavaScript debugger.
Searching for (and fixing) errors in programming code is called code debugging.
If your browser supports debugging, you can use console.log() to display JavaScript values in the debugger window:-
(the debugger statment) creates breakpoint where js will pause and let you look around.

========
Error Handling: Try...Catch
The try statement defines a code block to run (to try).
The catch statement defines a code block to handle any error.

Errors Will Happen!
When executing JavaScript code, different errors can occur.

Errors can be coding errors made by the programmer, errors due to wrong input, and other unforeseeable things.










=========================================




















