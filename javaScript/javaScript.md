<h1 style="font-family: Roboto" align="center">
JAVASCRIPT CHEAT SHEET
</h1>
<h3 style="font-family: Roboto">
Getting Started
</h3>

<h4 style="font-family: Roboto">
<code>Console </code> 
</h4>

```javascript
// => Hello world!
console.log('Hello world!');

// => Hello BMS
console.warn('hello %s', 'BMS');

// Prints error message to stderr
console.error(new Error('Oops!'));
```

<h4 style="font-family: Roboto">
<code>Numbers</code>
</h4>

```javascript
let amount = 6;
let price = 4.99;
```

<h4 style="font-family: Roboto">
<code>Variables</code>
</h4>

```javascript
let x = null;
let name = "Tammy";
const found = false;

// => Tammy, false, null
console.log(name, found, x);

var a;
console.log(a); // => undefined
```

<h4 style="font-family: Roboto">
<code>Strings</code> 
</h4>

```javascript
let single = 'Wheres my bandit hat?';
let double = "Wheres my bandit hat?";

// => 21
console.log(single.length);
```

<h4 style="font-family: Roboto">
<code>Arithmetic Operators</code>
</h4>

```javascript
5 + 5 = 10     // Addition
10 - 5 = 5     // Subtraction
5 * 10 = 50    // Multiplication
10 / 5 = 2     // Division
10 % 5 = 0     // Modulo
```

<h4 style="font-family: Roboto">
<code>Comments</code>
</h4>

```javascript
// This line will denote a comment

/*  
The below configuration must be 
changed before deployment. 
*/
```

<h4 style="font-family: Roboto">
<code>Assignment Operators</code>
</h4>

```javascript
let number = 100;

// Both statements will add 10
number = number + 10;
number += 10;

console.log(number); 
// => 120
```

<h4 style="font-family: Roboto">
<code>String Interpolation</code>
</h4>

```javascript
let age = 7;

// String concatenation
'Tommy is ' + age + ' years old.';

// String interpolation
`Tommy is ${age} years old.`;
```

<h4 style="font-family: Roboto">
<code>let Keyword</code>
</h4>

```javascript
let count; 
console.log(count); // => undefined
count = 10;
console.log(count); // => 10
```

<h4 style="font-family: Roboto">
<code>const Keyword</code>
</h4>

```javascript
const numberOfColumns = 4;

// TypeError: Assignment to constant...
numberOfColumns = 8;
```

<h3 style="font-family: Roboto">
JavaScript Conditionals 
</h3>

<h4 style="font-family: Roboto">
<code>if Statement</code>
</h4>

```javascript
const isMailSent = true;

if (isMailSent) {
  console.log('Mail sent to recipient');
}
```

<h4 style="font-family: Roboto">
<code>Ternary Operator</code>
</h4>

```javascript
var x=1;

// => true
result = (x == 1) ? true : false;
```

<h4 style="font-family: Roboto">
<code>Operators</code>
</h4>

```javascript
true || false;       // true
10 > 5 || 10 > 20;   // true
false || false;      // false
10 > 100 || 10 > 20; // false
```

<h5 style="font-family: Roboto">
<code>Logical Operator &&</code>
</h5>

```javascript
true && true;        // true
1 > 2 && 2 > 1;      // false
true && false;       // false
4 === 4 && 3 > 1;    // true
```

<h5 style="font-family: Roboto">
<code>Comparison Operators</code>
</h5>

```javascript
1 > 3                // false
3 > 1                // true
250 >= 250           // true
1 === 1              // true
1 === 2              // false
1 === '1'            // false
```

<h5 style="font-family: Roboto">
<code>Logical Operator !</code>
</h5>

```javascript
let lateToWork = true;
let oppositeValue = !lateToWork;

// => false
console.log(oppositeValue); // => false
```

<h5 style="font-family: Roboto">
<code>Nullish coalescing operator ??</code>
</h5>

```javascript
null ?? 'I win';           //  'I win'
undefined ?? 'Me too';     //  'Me too'

false ?? 'I lose'          //  false
0 ?? 'I lose again'        //  0
'' ?? 'Damn it'            //  ''
```

<h4 style="font-family: Roboto">
<code>else if</code>
</h4>

```javascript
const size = 10;

if (size > 100) {
  console.log('Big');
} else if (size > 20) {
  console.log('Medium');
} else if (size > 4) {
  console.log('Small');
} else {
  console.log('Tiny');
}
// Print: Small
```

<h4 style="font-family: Roboto">
<code>switch Statement</code>
</h4> 

```javascript
const food = 'salad';

switch (food) {
  case 'oyster':
    console.log('The taste of the sea');
    break;
  case 'pizza':
    console.log('A delicious pie');
    break;
  default:
    console.log('Enjoy your meal');
}
```

<h3 style="font-family: Roboto">
JavaScript Functions 
</h3>

<h4 style="font-family: Roboto">
<code>Functions</code>
</h4>

```javascript
// Defining the function:
function sum(num1, num2) {
  return num1 + num2;
}

// Calling the function:
sum(3, 6); // 9
```

<h4 style="font-family: Roboto">
<code>Anonymous Functions</code>
</h4>

```javascript
// Named function
function rocketToMars() {
  return 'BOOM!';
}

// Anonymous function
const rocketToMars = function() {
  return 'BOOM!';
}
```

<h4 style="font-family: Roboto">
<code>Arrow Functions (ES6)</code>
</h4>

```javascript
//With two arguments
const sum = (param1, param2) => { 
  return param1 + param2; 
}; 
console.log(sum(2,5)); // => 7 

//With no arguments
const printHello = () => { 
  console.log('hello'); 
}; 
printHello(); // => hello

//With a single argument
const checkWeight = weight => { 
  console.log(`Weight : ${weight}`); 
}; 
checkWeight(25); // => Weight : 25 

//Concise arrow functions
const multiply = (a, b) => a * b; 
// => 60 
console.log(multiply(2, 30)); 
```

<h4 style="font-family: Roboto">
<code>return Keyword</code>
</h4>

```javascript
// With return
function sum(num1, num2) {
  return num1 + num2;
}

// The function doesn't output the sum
function sum(num1, num2) {
  num1 + num2;
}
```

<h4 style="font-family: Roboto">
<code>Calling Functions</code>
</h4>

```javascript
// Defining the function
function sum(num1, num2) {
  return num1 + num2;
}

// Calling the function
sum(2, 4); // 6
```

<h4 style="font-family: Roboto">
<code>Function Expressions</code>
</h4>

```javascript
const dog = function() {
  return 'Woof!';
}
```

<h4 style="font-family: Roboto">
<code>Function Parameters</code>
</h4>

```javascript
// The parameter is name
function sayHello(name) {
  return `Hello, ${name}!`;
}
```

<h4 style="font-family: Roboto">
<code>Function Declaration</code>
</h4>

```javascript
function add(num1, num2) {
  return num1 + num2;
}
```

<h3 style="font-family: Roboto">
JavaScript Scope 
</h3>

<h4 style="font-family: Roboto">
<code>Scope</code>
</h4>

```javascript
function myFunction() {
  
  var pizzaName = "Margarita";
  // Code here can use pizzaName
  
}

// Code here can't use pizzaName
```

<h4 style="font-family: Roboto">
<code>Block Scoped Variables</code>
</h4>

```javascript
const isLoggedIn = true;

if (isLoggedIn == true) {
  const statusMessage = 'Logged in.';
}

// Uncaught ReferenceError...
console.log(statusMessage);
```

<h4 style="font-family: Roboto">
<code>Global Variables</code>
</h4>

```javascript
// Variable declared globally
const color = 'blue';

function printColor() {
  console.log(color);
}

printColor(); // => blue
```

<h3 style="font-family: Roboto">
JavaScript Arrays
</h3>

<h4 style="font-family: Roboto">
<code>Arrays</code>
</h4>

```javascript
const fruits = ["apple", "orange", "banana"];

// Different data types
const data = [1, 'chicken', false];
```

<h4 style="font-family: Roboto">
<code>Property .length</code>
</h4>

```javascript
const numbers = [1, 2, 3, 4];

numbers.length // 4
```

<h4 style="font-family: Roboto">
<code>Index</code>
</h4>

```javascript
// Accessing an array element
const myArray = [100, 200, 300];

console.log(myArray[0]); // 100
console.log(myArray[1]); // 200
```

<h4 style="font-family: Roboto">
<code>Method .push()</code>
</h4>

```javascript
// Adding a single element:
const cart = ['apple', 'orange'];
cart.push('pear'); 

// Adding multiple elements:
const numbers = [1, 2];
numbers.push(3, 4, 5); 
```

<h4 style="font-family: Roboto">
<code>Method .pop()</code>
</h4>

```javascript
const fruits = ["apple", "orange", "banana"];

const fruit = fruits.pop(); // 'banana'
console.log(fruits); // ["apple", "orange"]
```

<h4 style="font-family: Roboto">
<code>Method .shift()</code>
</h4>

```javascript
let cats = ['Bob', 'Willy', 'Mini'];

cats.shift(); // ['Willy', 'Mini']
```

<h4 style="font-family: Roboto">
<code>Method .unshift()</code>
</h4>

```javascript
let cats = ['Bob'];

// => ['Willy', 'Bob']
cats.unshift('Willy');

// => ['Puff', 'George', 'Willy', 'Bob']
cats.unshift('Puff', 'George');
```

<h4 style="font-family: Roboto">
<code>Method .concat()</code>
</h4>

```javascript
const numbers = [3, 2, 1]
const newFirstNumber = 4
    
// => [ 4, 3, 2, 1 ]
[newFirstNumber].concat(numbers)
    
// => [ 3, 2, 1, 4 ]
numbers.concat(newFirstNumber)
```

<h3 style="font-family: Roboto">
JavaScript Loops
</h3>

<h4 style="font-family: Roboto">
<code>While Loop</code>
</h4>

```javascript
while (condition) {
  // code block to be executed
}

let i = 0;
while (i < 5) {        
  console.log(i);
  i++;
}
```

<h4 style="font-family: Roboto">
<code>Reverse Loop</code>
</h4>

```javascript
const fruits = ["apple", "orange", "banana"];

for (let i = fruits.length - 1; i >= 0; i--) {
  console.log(`${i}. ${fruits[i]}`);
}

// => 2. banana
// => 1. orange
// => 0. apple
```

<h4 style="font-family: Roboto">
<code>Do…While Statement</code>
</h4>

```javascript
x = 0
i = 0

do {
  x = x + i;
  console.log(x)
  i++;
} while (i < 5);
// => 0 1 3 6 10
```

<h4 style="font-family: Roboto">
<code>For Loop</code>
</h4> 

```javascript
for (let i = 0; i < 4; i += 1) {
  console.log(i);
};

// => 0, 1, 2, 3
```

<h4 style="font-family: Roboto">
<code>Looping Through Arrays</code>
</h4>

```javascript
	for (let i = 0; i < array.length; i++){
  console.log(array[i]);
}

// => Every item in the array
```

<h4 style="font-family: Roboto">
<code>Break</code>
</h4>

```javascript
for (let i = 0; i < 99; i += 1) {
  if (i > 5) {
     break;
  }
  console.log(i)
}
// => 0 1 2 3 4 5
```

<h4 style="font-family: Roboto">
<code>Continue</code>
</h4>

```javascript
for (i = 0; i < 10; i++) {
  if (i === 3) { continue; }
  text += "The number is " + i + "<br>";
}
```

<h4 style="font-family: Roboto">
<code>Nested</code>
</h4>

```javascript
for (let i = 0; i < 2; i += 1) {
  for (let j = 0; j < 3; j += 1) {
    console.log(`${i}-${j}`);
  }
}
```

<h3 style="font-family: Roboto">
JavaScript Iterators 
</h3>

<h4 style="font-family: Roboto">
<code>Functions Assigned to Variables</code>
</h4>

```javascript
let plusFive = (number) => {
  return number + 5;  
};
// f is assigned the value of plusFive
let f = plusFive;

plusFive(3); // 8
// Since f has a function value, it can be invoked. 
f(9); // 14
```

<h4 style="font-family: Roboto">
<code>Callback Functions</code> 
</h4>

```javascript
const isEven = (n) => {
  return n % 2 == 0;
}

let printMsg = (evenFunc, num) => {
  const isNumEven = evenFunc(num);
  console.log(`${num} is an even number: ${isNumEven}.`)
}

// Pass in isEven as the callback function
printMsg(isEven, 4); 
// => The number 4 is an even number: True.
```

<h4 style="font-family: Roboto">
<code>Array Method .reduce()</code>
</h4>

```javascript
const numbers = [1, 2, 3, 4];

const sum = numbers.reduce((accumulator, curVal) => {  
  return accumulator + curVal;
});

console.log(sum); // 10
```

<h4 style="font-family: Roboto">
<code>Array Method .map()</code>
</h4>

```javascript
const members = ["Taylor", "Donald", "Don", "Natasha", "Bobby"];

const announcements = members.map((member) => {
  return member + " joined the contest.";
});

console.log(announcements);
```

<h4 style="font-family: Roboto">
<code>Array Method .forEach()</code>  
</h4>

```javascript
const numbers = [28, 77, 45, 99, 27];

numbers.forEach(number => {  
  console.log(number);
}); // => 28 77 45 99 27
```

<h4 style="font-family: Roboto">
<code>Array Method .filter()</code>
</h4>

```javascript
const randomNumbers = [4, 11, 42, 14, 39];
const filteredArray = randomNumbers.filter(n => {  
  return n > 5;
});
```

<h3 style="font-family: Roboto">
JavaScript Objects 
</h3>

<h4 style="font-family: Roboto">
<code>Accessing Properties</code>
</h4>

```javascript
const apple = { 
  color: 'Green',
  price: { bulk: '$3/kg', smallQty: '$4/kg' }
};
console.log(apple.color); // => Green
console.log(apple.price.bulk); // => $3/kg
```

<h4 style="font-family: Roboto">
<code>Naming Properties</code>
</h4>

```javascript
// Example of invalid key names
const trainSchedule = {
  // Invalid because of the space between words.
  platform num: 10, 
  // Expressions cannot be keys.
  40 - 10 + 2: 30,
  // A + sign is invalid unless it is enclosed in quotations.
  +compartment: 'C'
};
```

<h4 style="font-family: Roboto">
<code>Assignment shorthand syntax</code>
</h4>

```javascript
const person = {
  name: 'Tom',
  age: '22',
};
const {name, age} = person;
console.log(name); // 'Tom'
console.log(age);  // '22'
```

<h4 style="font-family: Roboto">
<code>Mutable</code>
</h4>

```javascript
const student = {
  name: 'Sheldon',
  score: 100,
  grade: 'A',
}

console.log(student)
// { name: 'Sheldon', score: 100, grade: 'A' }

delete student.score
student.grade = 'F'
console.log(student)
// { name: 'Sheldon', grade: 'F' }

student = {}
// TypeError: Assignment to constant variable.
```

<h4 style="font-family: Roboto">
<code>Delete operator</code>
</h4>

```javascript
const person = {
  firstName: "Matilda",
  age: 27,
  hobby: "knitting",
  goal: "learning JavaScript"
};

delete person.hobby; // or delete person[hobby];

console.log(person);
/*
{
  firstName: "Matilda"
  age: 27
  goal: "learning JavaScript"
}
*/
```

<h3 style="font-family: Roboto">
JavaScript Modules
</h3>

<h4 style="font-family: Roboto">  
<code>Export</code>
</h4>

```javascript
// myMath.js

// Default export
export default function add(x,y){
    return x + y
}

// Normal export
export function subtract(x,y){
    return x - y
}

// Multiple exports
function multiply(x,y){
    return x * y
}
function duplicate(x){
    return x * 2
}
export {
    multiply,
    duplicate
}
```

<h4 style="font-family: Roboto">
<code>Import</code>
</h4>

```javascript
// main.js
import add, { subtract, multiply, duplicate } from './myMath.js';

console.log(add(6, 2)); // 8 
console.log(subtract(6, 2)) // 4
console.log(multiply(6, 2)); // 12
console.log(duplicate(5)) // 10

// index.html
<script type="module" src="main.js"></script>
```

<h4 style="font-family: Roboto">
<code>Export Module</code>
</h4>

```javascript
// myMath.js

function add(x,y){
    return x + y
}
function subtract(x,y){
    return x - y
}
function multiply(x,y){
    return x * y
}
function duplicate(x){
    return x * 2
}

// Multiple exports in node.js
module.exports = {
    add,
    subtract,
    multiply,
    duplicate
}
```

<h4 style="font-family: Roboto">
<code>Require Module</code>
</h4>

```javascript
// main.js
const myMath = require('./myMath.js')

console.log(myMath.add(6, 2)); // 8 
console.log(myMath.subtract(6, 2)) // 4
console.log(myMath.multiply(6, 2)); // 12
console.log(myMath.duplicate(5)) // 10
```

<h3 style="font-family: Roboto">
JavaScript Promises 
</h3>

<h4 style="font-family: Roboto">
<code>Promise states</code>
</h4>

```javascript
const promise = new Promise((resolve, reject) => {
  const res = true;
  // An asynchronous operation.
  if (res) {
    resolve('Resolved!');
  }
  else {
    reject(Error('Error'));
  }
});

promise.then((res) => console.log(res), (err) => console.error(err));
```

<h4 style="font-family: Roboto">
<code>Executor function</code>
</h4>

```javascript
const executorFn = (resolve, reject) => {
  resolve('Resolved!');
};

const promise = new Promise(executorFn);
```

<h4 style="font-family: Roboto">
<code>setTimeout()</code>
</h4>

```javascript
const loginAlert = () =>{
  console.log('Login');
};

setTimeout(loginAlert, 6000);
```

<h4 style="font-family: Roboto">
<code>.then() method</code>
</h4>

```javascript
const promise = new Promise((resolve, reject) => {    
  setTimeout(() => {
    resolve('Result');
  }, 200);
});

promise.then((res) => {
  console.log(res);
}, (err) => {
  console.error(err);
});
```

<h4 style="font-family: Roboto">
<code>.catch() method</code>
</h4>

```javascript
const promise = new Promise((resolve, reject) => {  
  setTimeout(() => {
    reject(Error('Promise Rejected Unconditionally.'));
  }, 1000);
});

promise.then((res) => {
  console.log(value);
});

promise.catch((err) => {
  console.error(err);
});
```

<h4 style="font-family: Roboto">
<code>Promise.all()</code>
</h4>

```javascript
const promise1 = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve(3);
  }, 300);
});
const promise2 = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve(2);
  }, 200);
});

Promise.all([promise1, promise2]).then((res) => {
  console.log(res[0]);
  console.log(res[1]);
});
```

<h4 style="font-family: Roboto">
<code>Creating</code>
</h4>

```javascript
const executorFn = (resolve, reject) => {
  console.log('The executor function of the promise!');
};

const promise = new Promise(executorFn);
```

<h3 style="font-family: Roboto">
JavaScript Async-Await 
</h3>

<h4 style="font-family: Roboto">
<code>Asynchronous</code>
</h4>

```javascript
function helloWorld() {
  return new Promise(resolve => {
    setTimeout(() => {
      resolve('Hello World!');
    }, 2000);
  });
}

async function msg() {
  const msg = await helloWorld();
  console.log('Message:', msg);
}

msg(); // Message: Hello World! <-- after 2 seconds
```

<h4 style="font-family: Roboto">
<code>Error Handling</code>
</h4>

```javascript
let json = '{ "age": 30 }'; // incomplete data

try {
  let user = JSON.parse(json); // <-- no errors
  console.log( user.name ); // no name!
} catch (e) {
  console.error( "Invalid JSON data!" );
}
```

<h4 style="font-family: Roboto">
<code>Aysnc await operator</code>
</h4>

```javascript
function helloWorld() {
  return new Promise(resolve => {
    setTimeout(() => {
      resolve('Hello World!');
    }, 2000);
  });
}

async function msg() {
  const msg = await helloWorld();
  console.log('Message:', msg);
}

msg(); // Message: Hello World! <-- after 2 seconds
```

<h3 style="font-family: Roboto">
JavaScript Requests
</h3>

<h4 style="font-family: Roboto">
<code>JSON</code>
</h4>

```javascript
const jsonObj = {
  "name": "Rick",
  "id": "11A",
  "level": 4  
};
```

<h4 style="font-family: Roboto">
<code>XMLHttpRequest</code>
</h4>

```javascript
const xhr = new XMLHttpRequest();
xhr.open('GET', 'mysite.com/getjson');
```

<h4 style="font-family: Roboto">
<code>GET</code>
</h4>

```javascript
const req = new XMLHttpRequest();
req.responseType = 'json';
req.open('GET', '/getdata?id=65');
req.onload = () => {
  console.log(xhr.response);
};

req.send();
```

<h4 style="font-family: Roboto">
<code>POST</code>
</h4>

```javascript
const data = {
  fish: 'Salmon',
  weight: '1.5 KG',
  units: 5
};
const xhr = new XMLHttpRequest();
xhr.open('POST', '/inventory/add');
xhr.responseType = 'json';
xhr.send(JSON.stringify(data));

xhr.onload = () => {
  console.log(xhr.response);
};
```

<h4 style="font-family: Roboto">
<code>fetch api</code>
</h4>

```javascript
fetch(url, {
    method: 'POST',
    headers: {
      'Content-type': 'application/json',
      'apikey': apiKey
    },
    body: data
  }).then(response => {
    if (response.ok) {
      return response.json();
    }
    throw new Error('Request failed!');
  }, networkError => {
    console.log(networkError.message)
  })
}
```

<h4 style="font-family: Roboto">
<code>JSON Formatted</code>
</h4>

```javascript
fetch('url-that-returns-JSON')
.then(response => response.json())
.then(jsonResponse => {
  console.log(jsonResponse);
});
```

<h4 style="font-family: Roboto">
<code>promise url parameter fetch api</code>
</h4>

```javascript
fetch('url')
.then(
  response  => {
    console.log(response);
  },
 rejection => {
    console.error(rejection.message);
);
```

<h4 style="font-family: Roboto">
<code>Fetch API Function</code>
</h4>

```javascript
fetch('https://api-xxx.com/endpoint', {
  method: 'POST',
 body: JSON.stringify({id: "200"})
}).then(response => {
  if(response.ok){
	  return response.json();  
  }
	throw new Error('Request failed!');
}, networkError => {
  console.log(networkError.message);
}).then(jsonResponse => {
  console.log(jsonResponse);
});
```

<h4 style="font-family: Roboto">
<code>async await syntax</code>
</h4>

```javascript
const getSuggestions = async () => {
  const wordQuery = inputField.value;
  const endpoint = `${url}${queryParams}${wordQuery}`;
  try{
const response = await fetch(endpoint, {cache: 'no-cache'});
    if(response.ok){
      const jsonResponse = await response.json()
    }
  }
  catch(error){
    console.log(error)
  }
}
```