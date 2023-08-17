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
============================






















