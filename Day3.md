OBJECT:
let obj={name:"aya",age:22};
typeOf(obj);==>object
note: typeof ["aya"];==>object
["aya"].length==>1
========================================
object methods:-
let obj= {
name:"aya",
age:22,
fun:function(){
console.log("yes")
}
}

obj.fun();===>"yes"
obj.name;==>aya
=============================================
**this in a method referance to properites in object
EXAMPLE:-
let obj= {
name:"aya"
}
obj.age=function(){
console.log("my name is",this.name)
}

obj.age();==>my name is aya
===================================================
Nested object:-
Example:
let obj= {
obj1:
{
name:"aya",
age:22,
},
obj2:
{name:"sara",
age:25,
}
};

obj.obj1.name;==>aya
=======================================================
Objects in array:-
const arr=[
{name:"aya",
age:24,},

{name:"sara",
age:22,},

{name:"haya",
age:26,}
]
=============================================
console.log("aya");//print aya
console.warn("aya");
console.error("aya");
=============================================
Math:
Math.random();//between 0-1
Math.PI();==>3.14
Math.abs(-5);==>5
=============================================
String methods:
"aya".length==>3
"aya".toUpperCase()==>AYA
===============================================
Quiz Project:-
string immutable we cant edited in it.
important note*****typeof['a']===>object
typeof['a']==='array';False

in HTML DOC we write js in <script> element.
to make comments in js we use (//).

let x={
'name':"aya",
}

x['name'];==>'aya'.




