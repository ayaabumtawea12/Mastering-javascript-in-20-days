## closure:
A closure is a feature of JavaScript that allows inner functions to access the outer scope of a function. Closure helps in binding a function to its outer boundary and is created automatically whenever a function is created. A block is also treated as a scope since ES6. Since JavaScript is event-driven so closures are useful as it helps to maintain the state between events.

function foo() {
    let b = 1;
    function inner() {
        return b;
    }
    return inner;
}
let get_func_inner = foo();//nested function scope
 console.log(get_func_inner());

![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/2e894db3-59e0-458d-8bd7-b5aac4e5bd76)
===========================================================
## Async js:-
Functions running in parallel with other functions are called asynchronous
A good example is JavaScript setTimeout()

setTimeout(myFunction, 3000);

function myFunction() {
  document.getElementById("demo").innerHTML = "I love You !!";
}

In the example above, myFunction is used as a callback.

myFunction is passed to setTimeout() as an argument.

3000 is the number of milliseconds before time-out, so myFunction() will be called after 3 seconds.
=========================================================
![image](https://github.com/ayaabumtawea12/Mastering-javascript-in-20-days/assets/120716752/5818886e-e1be-4de7-ae19-6fdd1df8a899)
===================================
## Q1:-
You are given a function executeInSequenceWithCBs and some code. The task is to modify the executeInSequenceWithCBs function so that it runs and executes all the tasks inside the asyncTasks array.
The function should return an array of messages obtained from each task's execution.
You are only allowed to change the executeInSequenceWithCBs function or add new functions/code. You cannot modify the tasks' functions.


const task1 = (cb) => setTimeout(() => {
  const message = "Task 1 has executed successfully!";
  cb(message);
}, 3000)

const task2 = (cb) => setTimeout(() => {
  const message = "Task 2 has executed successfully!";
  cb(message);
}, 0)

const task3 = (cb) => setTimeout(() => {
  const message = "Task 3 has executed successfully!";
  cb(message);
}, 1000)

const task4 = (cb) => setTimeout(() => {
  const message = "Task 4 has executed successfully!";
  cb(message);
}, 2000)

const task5 = (cb) => setTimeout(() => {
  const message = "Task 5 has executed successfully!";
  cb(message);
}, 4000)

const asyncTasks = [task1, task2, task3, task4, task5];

const executeInSequenceWithCBs = (tasks, callback) => {}





















