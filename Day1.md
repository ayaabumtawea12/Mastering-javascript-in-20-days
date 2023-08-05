we can write js in :
1-browser.
2-text file like vs code.
======================
DOM IN JS: s a standard object model and programming interface for HTML.
======================
document.getElementById("x")//return first element with id=x.
document.querySelector("#x")//return first element with id=x.
document.getElementsByTagName("x")//return all x elements.
document.querySelectorAll("x")//return all x elements.
document.getElementsByClassName("x")//return all elements with classnamae x.
document.querySelectorAll(".x")//return all elements with class name = x.
===============================================
document.getElementsByClassName("x").length//return number of element who class name x
document.getElementById("x").textContent//return text inside element with id=x; 
document.getElementById("x").textContent="ahusu"//change text content
document.getElementById("x").append="ahusu"//add text to text content
===============================================
Data type
1-string("aya","24");
EXample:
let x="24"
typeof(x)//string
typeof//tell you type of value.

2-number
EXample:25,2.5
let x=24;

typeof(x)//number

3-bool
===============
***JS has two type of data:-
1-primitave data like string,num,bool,undefined,null.
let x;
console.log(x);=>undefined;
let x=null;
console.log(x)=>null

2-object data like document.
==========================
STRING:-
"aya".length =>3
" ".length =>1
================================================
***INDEX
let x='aya'
x[0]=>a;
--------
"Aya".indexOf('A')=>0
"Aya".indexOf('Q')=>-1
"Aya".includes('Ay')=>true
"Aya".startWith('A')=>true
"Aya".indexOf('Ay')=>0
"Aya".indexOf('ys')=>-1
"Aya"+"12"==>Aya12
"Aya".toLowerCase()=>"aya"
=======================================================================
*****OPERATORS:
(+) this op use to connect string or to calculate
"aya" +"as"=>'ayaas'

--Arthmetic operators (/ * - + )
Sort by priority( (),/ * ,-+)
(4+1)*2=>10
1*6+4=>10

******comparation operator(> greater,< smaller,>=,<=);
5>4==>true





=========================================================================
Tasks-:
task 1-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/compound-assignment-with-augmented-multiplication
a should equal 25.
Waiting:b should equal 36.
Waiting:c should equal 46.
Waiting:You should use the *= operator for each variable.
Waiting:You should not modify the code above the specified comment.

let a = 5;
let b = 12;
let c = 4.6;

// Only change code below this line
a *= 5;
b *= 3;
c *= 10;

====================================================
task 2-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/concatenating-strings-with-the-plus-equals-operator
myStr should have a single space character between the two strings.
Passed:myStr should have a value of the string This is the first sentence. This is the second sentence.
Passed:You should use the += operator to build myStr.

let myStr="This is the first sentence.";
myStr +=" This is the second sentence."
==================================
task 3-https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-bracket-notation-to-find-the-nth-to-last-character-in-a-string

secondToLastLetterOfLastName should be the letter c.
Passed:You should use .length to get the second last letter.

const lastName = "Lovelace";
const secondToLastLetterOfLastName = lastName[lastName.length - 2];
===============================================
//Assigning and declaration  a variable
let x;//declaration variable
x="aya";//Assigning a variable
===============================================
