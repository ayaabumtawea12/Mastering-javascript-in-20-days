conditionals:-
if(4>5){
console.log("yes");
}else if(4>2){
console.log("hi");
}else{
console.log("no");
}
======================
if(1){
    console.log("4");
}===>4

if(0){
    console.log("4");
}//undefined
============================
Exercise:
let fistname="aya";
let lastname="abu mtawea";

if(firstname.length>lastname.length)
{
console.log(firstname+"is longer than"+lastname);
}else{
console.log(lastname+"is longer than"+ firstname);
}
==============================================
function arr(array){
if(array.length === 0){
return true
} else{
return false;
}

arr([1,2,3])==>false
===============================================
if([])
{
console.log("true");
}=====>true

====================
if("")
{
console.log("true");
}else{
console.log("false");
}=====>false
=========================
if(null)
{
console.log("true");
}else{
console.log("false");
}=====>false
*****
if(undefined)
{
console.log("true");
}else{
console.log("false");
}=====>false
============================
if("false")
{
console.log("true");
}else{
console.log("false");
}=====>true
================================**********************************===================================
Logical:= and=> && **   or=>|| 
Ternary operator:-   condition ? valueiftrue : valueiffalse  =>for write quick condition 
if(x==3)                               
{                        equevalent       x==3 ?"yes":"no";
console.log("yes");
}else{
console.log("no");
}
}
=================================================================================
Loop:
let number=[1,2,3];
for(let x=0 ;x<number.length; x++)
{
console.log(number[x]);
}

for(let n of number){
console.log(n) ==>1 2 3
}
======================================================================================
for(let n of "aya"){
console.log(n) ==>a y a
}
================================================================
Map & Filter:-
Map:=> calls a function on each item in an array to create a new array
arrow function useful for this.

const numbers = [1, 2, 3, 4];
const doubled = numbers.map(item => item * 2);

filter: =>method takes each element in an array and it applies a conditional statement against it

const numbers = [1, 2, 3, 4];
const evens = numbers.filter(item => item % 2 === 0);
console.log(evens); // [2, 4]
============================================================
**Spread: we use it to put all item  from one array inside another array
let x=[1,2,3]
let y=[4,5,6]

let w=[...x,...y]; equivelent  let z=x.concat(y);
===========================================================
Array are like object?//true
===========================================================
While loop:-
let x=[];
while(x.length<5){
x.push(Math.random());
}
================================
settimeout: async code 
code that take a long time.
settimeout(()=> conole.log("time"),1000); //tiis code execute after 1s.
=============================
===========================================================
Q1:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-multiple-conditional-ternary-operators
function checkSign(num) {
return num > 0 ? "positive" : num < 0 ? "negative" : "zero";
}

checkSign(10);
====================================
Q2:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-map-method-to-extract-data-from-an-array
// The global variable
const watchList = [
  {
  ........
  }
];

// Only change code below this line
let ratings=watchList.map(movie=>{
  let refinedMovieData={};
  refinedMovieData["title"]=movie["Title"];
  refinedMovieData["rating"]=movie["imdbRating"]
  return refinedMovieData;
})
 

// Only change code above this line

console.log(JSON.stringify(ratings));
================================================================
Q3:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-filter-method-to-extract-data-from-an-array
// The global variable
const watchList = [
  {
    "Title": "Inception",
    "Year": "2010",
    "Rated": "PG-13",
    "Released": "16 Jul 2010",
    "Runtime": "148 min",
    "Genre": "Action, Adventure, Crime",
    "Director": "Christopher Nolan",
    "Writer": "Christopher Nolan",
    "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Elliot Page, Tom Hardy",
    "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
    "Language": "English, Japanese, French",
    "Country": "USA, UK",
    "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
    "Metascore": "74",
    "imdbRating": "8.8",
    "imdbVotes": "1,446,708",
    "imdbID": "tt1375666",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "Interstellar",
    "Year": "2014",
    "Rated": "PG-13",
    "Released": "07 Nov 2014",
    "Runtime": "169 min",
    "Genre": "Adventure, Drama, Sci-Fi",
    "Director": "Christopher Nolan",
    "Writer": "Jonathan Nolan, Christopher Nolan",
    "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
    "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
    "Language": "English",
    "Country": "USA, UK",
    "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
    "Metascore": "74",
    "imdbRating": "8.6",
    "imdbVotes": "910,366",
    "imdbID": "tt0816692",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "The Dark Knight",
    "Year": "2008",
    "Rated": "PG-13",
    "Released": "18 Jul 2008",
    "Runtime": "152 min",
    "Genre": "Action, Adventure, Crime",
    "Director": "Christopher Nolan",
    "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
    "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
    "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
    "Language": "English, Mandarin",
    "Country": "USA, UK",
    "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
    "Metascore": "82",
    "imdbRating": "9.0",
    "imdbVotes": "1,652,832",
    "imdbID": "tt0468569",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "Batman Begins",
    "Year": "2005",
    "Rated": "PG-13",
    "Released": "15 Jun 2005",
    "Runtime": "140 min",
    "Genre": "Action, Adventure",
    "Director": "Christopher Nolan",
    "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
    "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
    "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
    "Language": "English, Urdu, Mandarin",
    "Country": "USA, UK",
    "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
    "Metascore": "70",
    "imdbRating": "8.3",
    "imdbVotes": "972,584",
    "imdbID": "tt0372784",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "Avatar",
    "Year": "2009",
    "Rated": "PG-13",
    "Released": "18 Dec 2009",
    "Runtime": "162 min",
    "Genre": "Action, Adventure, Fantasy",
    "Director": "James Cameron",
    "Writer": "James Cameron",
    "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
    "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
    "Language": "English, Spanish",
    "Country": "USA, UK",
    "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
    "Metascore": "83",
    "imdbRating": "7.9",
    "imdbVotes": "876,575",
    "imdbID": "tt0499549",
    "Type": "movie",
    "Response": "True"
  }
];

// Only change code below this line

const filteredList = watchList.map(list=>{
  let object={};
  object.title=list.Title;
  object.rating=list.imdbRating;

  return object;
}).filter(list=>{
  let ratingInt=parseFloat(list.rating);

  if(ratingInt >= 8){
    return list;
  }
})

// Only change code above this line

console.log(filteredList);



=======
Q4:
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/golf-code
const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

function golfScore(par, strokes) {
  // Only change code below this line
if(strokes === 1){
return "Hole-in-one!";
} else if(strokes <= par-2)
{
return "Eagle";
} else if(strokes <= par-1)
{
return "Birdie";
} else if(strokes === par)
{
return "Par";
}
else if(strokes === par+1)
{
return "Bogey";
}
else if(strokes === par+2)
{
return "Double Bogey";
}
else if(strokes >= par+3)
{
return "Go Home!";
}

  return "Change Me";
  // Only change code above this line
}

golfScore(5, 4);
==================











