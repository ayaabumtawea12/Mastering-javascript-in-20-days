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
 











=========================================




















