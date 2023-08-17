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

