function  print() {
console.log("hi");
} 
setTimeout(print,0); 
console.log("hello");
result==>hello
         hi
============================
## callback funcion:-
- A callback is a function passed as an argument to another function.
- This technique allows a function to call another function.
- A callback function can run after another function has finished.
  
<p id="demo"></p>
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}

function myFirst() {
  myDisplayer("Hello");
}

function mySecond() {
  myDisplayer("Goodbye");
}

myFirst();
mySecond();
===============================
## Promises:-
"Producing code" is code that can take some time.
"Consuming code" is code that must wait for the result.
A Promise is a JavaScript object that links producing code and consuming code
A JavaScript Promise object contains both the producing code and calls to the consuming code.

let myPromise = new Promise(function(myResolve, myReject) {
  setTimeout(function() { myResolve("I love You !!"); }, 3000);
});

myPromise.then(function(value) {
  document.getElementById("demo").innerHTML = value;
})
==================================
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/d99f0eec-b306-479a-a8ed-4caf52167bcb)
==================================
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/b34b8cea-3098-4e27-a8e0-00b05cd5e9f6)
==================================















