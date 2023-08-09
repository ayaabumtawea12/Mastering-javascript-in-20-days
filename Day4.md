Function:-
to create function:-
function half(x){
return x;
}
to call function:-
half(5);
========================================
Parametars & arguments:
function add(x,y,z//x,y,z these are parametars(the inputs a function expects);
console.log("x","y","z");
}
add(1,2,3);//1,2,3  these are arguments (actual value the function is called with)
===============================================
parameters should be named like variables and beheve like a variable within the function body
================================================
**note: 1+undefined=>NaN
typeof(NaN)==>number
0/0==>NaN
================================================
function add()
{
return Math.random();
}
add("unexpected");===>0.12658545
=======================================================
function squere(x)
{
console.log(x*x);
}
let sq=squere(3);==>9
sq;==>undefined
========================================================
///important note:-
function squere(x)
{
console.log(x*x);
return x*x;
}
let sq=squere(3);==>9
sq;==>9 
=====================================================
function squere(x)
{
return x*x;
console.log(x*x);
}
let sq=squere(3);==>udefined
sq;==>9 
======================================================
Arrow function:-
function add(x,y){
return x;
}
OR 
let A=(x,y)=> x+y;
A(1,2);
=====================================================
const print=(text)=>console.log(text.toLowerCase());
print("AYA");==>aya
let w=print("AYA");//undefined
w;=>aya
=====================================================
SetAttribute:
<button name="aya" value="true">
b.SetAttribute("name","asd");
b.SetAttribute("disabled")//error
b.SetAttribute("disabled"," ");
b.removeAttribute("disabled")
============================================
Scope:-
what variable and where we declare variable

let x=4;
function add(){
x=5;
}
x;=>4
add()
x;==>5//when execute function x become 5
============================================
Events and handler:
document.AddEventListener("click",() => {
console.log("clocked");
});

document.AddEventListener("click",(event) => {
console.log(event);

h1.AddEventListener("mouseout",() => {
 h1.textcontent="aya";
});

click,mouseover,mouseout,dbclick,.....
=====================


















