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
## Question 1(Exercises for Async JS & Promises):-

https://github.com/orjwan-alrajaby/gsg-QA-Nablus-training-2023/blob/main/learning-sprint-1/week2%20-%20javaScript-the-hard-parts-v2/day%203/tasks.md

You are given a function executeInSequenceWithCBs and some code. The task is to modify the executeInSequenceWithCBs function so that it runs and executes all the tasks inside the asyncTasks array.
The function should return an array of messages obtained from each task's execution.
You are only allowed to change the executeInSequenceWithCBs function or add new functions/code. You cannot modify the tasks' functions.

##solution:-

const task1 = () => new Promise((resolve) => {
    setTimeout(() => {
      const message = "Task 1 has executed successfully!";
      resolve(message);
    }, 3000);
  });

  const task2 = () => new Promise((resolve) => {
    setTimeout(() => {
      const message = "Task 2 has executed successfully!";
      resolve(message);
    }, 0);
  });

  const task3 = () => new Promise((resolve) => {
    setTimeout(() => {
      const message = "Task 3 has executed successfully!";
      resolve(message);
    }, 1000);
  });

  const task4 = () => new Promise((resolve) => {
    setTimeout(() => {
      const message = "Task 4 has executed successfully!";
      resolve(message);
    }, 2000);
  });

  const task5 = () => new Promise((resolve) => {
    setTimeout(() => {
      const message = "Task 5 has executed successfully!";
      resolve(message);
    }, 4000);
  });

  const asyncTasks = [task1, task2, task3, task4, task5];

  const executeInSequenceWithCBs = async (tasks, callback) => {
    const promises = tasks.map((task) => task());
    const results = await Promise.all(promises);
    callback(results);
    return results;
  };

  executeInSequenceWithCBs(asyncTasks, (messages) => {
    console.log(messages);
  });

=============================================================================
## Question 2:
You are given a function called executeInParallelWithPromises, which takes an array of APIs (represented by objects).

Your task is to write code that fetches the data of each API in parallel using promises. In Parallel means that the api which resolves first, returns its value first, regardless of the execution order.

The output of the executeInParallelWithPromises function should be an array containing the results of each API's execution.

Each result should be an object with three keys: apiName, apiUrl, and apiData..

##solution:-
const apis = [
  {
    apiName: "products", 
    apiUrl: "https://dummyjson.com/products",
  }, 
  {
    apiName: "users", 
    apiUrl: "https://dummyjson.com/users",
  }, 
  {
    apiName: "posts", 
    apiUrl: "https://dummyjson.com/posts",
  }, 
  {
    apiName: "comments", 
    apiUrl: "https://dummyjson.com/comments",
  }
];

const executeInParallelWithPromises = (apis) => {
    const promises = apis.map(api => {
        return fetch(api.apiUrl) .then(response => { response.json() }) .then(data => {
         return {
          apiName: api.apiName,
          apiUrl: api.apiUrl,
          apiData: data
                }
            })
    })

    return Promise.all(promises)
}

executeInParallelWithPromises(apis)
.then(data=>console.log(data))
.catch(error => console.log(error));
=============================================
## Question 3:-
ou are given a function called executeInSequenceWithPromises, which takes an array of APIs (represented by objects).

Your task is to write code that fetches the data of each API sequentially (one after the other) using promises.

In Sequence means that the api which executes first, returns its value first.

The output of the executeInSequenceWithPromises function should be an array containing the results of each API's execution.

Each result should be an object with three keys: apiName, apiUrl, and apiData.

const apis = [
  {
    apiName: "products", 
    apiUrl: "https://dummyjson.com/products",
  }, 
  {
    apiName: "users", 
    apiUrl: "https://dummyjson.com/users",
  }, 
  {
    apiName: "posts", 
    apiUrl: "https://dummyjson.com/posts",
  }, 
  {
    apiName: "comments", 
    apiUrl: "https://dummyjson.com/comments",
  }
]

//modify and write your code here
const executeInSequenceWithPromises = async (apis) => {
    const results = [];
    for (let api of apis){
    const respose = await fetch(api.apiUrl)
    const data = await respose.json();
    results.push({
    apiName: api.apiName,
    apiUrl: api.apiUrl,
    apiData: data
    })
    }
    return results;
}

executeInSequenceWithPromises(apis)
.then(results=>{console.log(results)
})
.catch(error =>{
console.log(error)
})


















