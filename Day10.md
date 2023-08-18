## Classes && prototypes:
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/69942fd6-18af-4e36-8402-2dd01c1a1f97)
=============
## object dot notation:-
let student{
name:'aya',
age:9,
score:funnction(){
console.log("pass")
console.log(student.name);

}
};

student.age;==>5
student.score();==>'pass'
                   'aya'
==================================
create empty object and add prop by dot notation.
let student{}//empty object


student.age=5;
student.score=funnction(){
console.log("pass");
console.log(student.name);
}
==========================
## factory functions in JavaScript:-
-The Factory Function is similar to constructor functions/class functions, but instead of using new to create an object, factory functions simply creates an object and returns it.

-they do not require the use of the ‘this‘ keyword for inner values or the use of the ‘new‘ keyword when instantiating new objects


// Function creating new objects 
// without use of 'new' keyword
    function createRobot(name) {
        return {
            name: name,
            talk: function () {
                console.log('My name is ' 
                + name + ', the robot.');
            }
        };
    }
  
    //Create a robot with name Chitti
    const robo1 = createRobot('Chitti');
  
    robo1.talk();
===========================================================
## prototype chain:
object.create();
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/ad001510-30af-41b7-9744-45e0ca6573d7)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/6219246f-61a7-4fee-b948-b1dfd1587967)
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/7abd389d-d69b-4a00-b8b2-ddb4d677954f)
=============================
## hasOwnProperty()
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/a91ff11b-d2ca-4f24-99e1-bf6affa46e5a)
onst object1 = {};
object1.property1 = 42;

console.log(object1.hasOwnProperty('property1'));
// Expected output: true

console.log(object1.hasOwnProperty('toString'));
// Expected output: false

console.log(object1.hasOwnProperty('hasOwnProperty'));
// Expected output: false
==========================================
## this Keyword:-
In JavaScript, the this keyword refers to an object .
const person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }


The this keyword refers to different objects depending on how it is used:
***notes:-
1-In an object method, this refers to the object.
2-Alone, this refers to the global object.//window object
3-In a function, this refers to the global object.
4-In a function, in strict mode, this is undefined.
5-In an event, this refers to the element that received the event.
6-Methods like call(), apply(), and bind() can refer this to any object.

**this is not a variable. It is a keyword. You cannot change the value of this.
============================

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/edb9fca9-5f74-463b-92e6-f66051c0665f)
=============================
## New keyword:-
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/fd41b5e7-6d55-4b50-8b26-31f00a177177)
=======================
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/6543ac2f-e6fa-49d7-a53d-b05582cd6b4b)
==============================
## classes:-
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/cad0879c-8dc4-4d2c-92ce-1b69ffde26b2)
******note 
function Bird(name) {
  this.name = name;
}
let duck = new Bird("Donald");
duck inherits its prototype from the Bird constructor function. You can show this relationship with the isPrototypeOf method:

Bird.prototype.isPrototypeOf(duck);
This would return true.
/////
All objects in JavaScript (with a few exceptions) have a prototype. Also, an object’s prototype itself is an object.

function Bird(name) {
  this.name = name;
}
Because a prototype is an object, a prototype can have its own prototype! In this case, the prototype of Bird.prototype is Object.prototype:

Object.prototype.isPrototypeOf(Bird.prototype);
====
** Bird.prototype.constructor=Bird;
==============
## Set the Child's Prototype to an Instance of the Parent

function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};

function Dog() { }

// Only change code below this line


let beagle = new Dog();
Dog.prototype = Object.create(Animal.prototype);//inheritance
====================
function Bird() { }

Bird.prototype.fly = function() { return "I am flying!"; };

function Penguin() { }
Penguin.prototype = Object.create(Bird.prototype);
Penguin.prototype.constructor = Penguin;
===================
function Bird() {
let weight = 15;//private 

this.getWeight = function() { 
    return weight;
  };

}
====================
## important things
A common pattern in JavaScript is to execute a function as soon as it is declared:
(function () {
  console.log("A cozy nest is ready");
})();//This is an anonymous function expression that executes right away--This pattern is known as an immediately invoked function expression or IIFE. function without name.
===================




==============================
## Question 1:-
## Object Oriented Programming
https://github.com/orjwan-alrajaby/gsg-QA-Nablus-training-2023/blob/main/learning-sprint-1/week2%20-%20javaScript-the-hard-parts-v2/day%204/task.md

My Profile: https://www.freecodecamp.org/Aya_Abu_Mtawea

1 ## https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/create-a-basic-javascript-object
2-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-dot-notation-to-access-the-properties-of-an-object
3-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/create-a-method-on-an-object
4-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/make-code-more-reusable-with-the-this-keyword
5-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/define-a-constructor-function
6-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-a-constructor-to-create-objects
7-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/extend-constructors-to-receive-arguments

8-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/verify-an-objects-constructor-with-instanceof

9-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/understand-own-properties
10-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-prototype-properties-to-reduce-duplicate-code

11-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/iterate-over-all-properties
12-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/understand-the-constructor-property
13-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/change-the-prototype-to-a-new-object
14-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/remember-to-set-the-constructor-property-when-changing-the-prototype
15-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/understand-where-an-objects-prototype-comes-from
16-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/understand-the-prototype-chain
17-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-inheritance-so-you-dont-repeat-yourself
18-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/inherit-behaviors-from-a-supertype
19-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/set-the-childs-prototype-to-an-instance-of-the-parent
*20-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/reset-an-inherited-constructor-property
21-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/add-methods-after-inheritance
22-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/override-inherited-methods
23-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-a-mixin-to-add-common-behavior-between-unrelated-objects
24-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-closure-to-protect-properties-within-an-object-from-being-modified-externally
25-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/understand-the-immediately-invoked-function-expression-iife
26-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/object-oriented-programming/use-an-iife-to-create-a-module
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/4660a8df-dfeb-4d27-a58c-52dbc7d12774)













