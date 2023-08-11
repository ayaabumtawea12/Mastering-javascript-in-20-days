Fetching data:
APIs provides a URL that point at data we care about.
fetch("url......") load data from API;
it take time to fetch data from network.....

A-Promises
can be in 3 possible states:
1-pending
2-fufilled
3-rejected

B-A wait 
lets us tell js to stop and wait for an async operation to finish.

let response=await fetch("...")
console.log(response);

let body= await response.json();//return data ;
fetch(" ").then((value)=>console.log(value));
===========================================================
