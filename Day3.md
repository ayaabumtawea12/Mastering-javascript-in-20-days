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

==============================================================================
QUESTION1:-
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-data-structures/copy-array-items-using-slice
function forecast(arr) {
  // Only change code below this line
  arr.slice(2, 4);
  return arr;
}

// Only change code above this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
result==>['warm', 'sunny']
==========================================================================================
QUESTION2:-
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-data-structures/combine-arrays-with-the-spread-operator
Combine Arrays with the Spread Operator
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence=["learning",...fragment,"is", "fun"]; // Change this line
  return sentence;
}

console.log(spreadOut());
===========================================================================================
QUESTION3:-
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/profile-lookup
// Setup
const contacts = [
  {
    firstName: "Akira",
    lastName: "Laine",
    number: "0543236543",
    likes: ["Pizza", "Coding", "Brownie Points"],
  },
  {
    firstName: "Harry",
    lastName: "Potter",
    number: "0994372684",
    likes: ["Hogwarts", "Magic", "Hagrid"],
  },
  {
    firstName: "Sherlock",
    lastName: "Holmes",
    number: "0487345643",
    likes: ["Intriguing Cases", "Violin"],
  },
  {
    firstName: "Kristian",
    lastName: "Vos",
    number: "unknown",
    likes: ["JavaScript", "Gaming", "Foxes"],
  },
];

function lookUpProfile(name, prop) {
  // Only change code below this line
for(var i=0; i<contacts.length;i++){
  if(contacts[i]['firstName'] === name)
  {
    if(contacts[i].hasOwnProperty(prop)){
      return contacts[i][prop];
    } else{
      return 'No such property';
    }
  }
}
return 'No such contact';
  // Only change code above this line
}
console.log(lookUpProfile("sherlock","number"));
lookUpProfile("Akira", "likes");
=============================================================================================
QUESTION 4:-
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/write-reusable-javascript-with-functions
function reusableFunction(){
  console.log("Hi World")
}

reusableFunction();
================================================================================================
QUESTION 5:-
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/understanding-undefined-value-returned-from-a-function
// Setup
let sum = 0;

function addThree() {
  sum = sum + 3;
}

addThree() 
// Only change code below this line
console.log(sum)

function addFive(){
  sum=sum+5;
}
// Only change code above this line

 
var value=addFive();

console.log(sum)
==============================================================
QUESTION 6:-
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/understanding-undefined-value-returned-from-a-function

function seven(num)
{
  return num-7;
}

function timesFive (num){
 return num*5;
}

console.log(seven(10))
console.log(timesFive(5))
console.log(timesFive(2))
console.log(timesFive(0))


