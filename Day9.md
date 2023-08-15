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
