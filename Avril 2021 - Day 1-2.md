# Coding-diary
Everyday learning

[Friday 2nd of April](2021-04/02.md)

[Monday 5th of April] (2021-04/02.md)

JavaScript

——————————

OBJECT PRIMITIVE
———————————

petite fonctions de base :

const s= [“a, b, c, d”]

console.log(const.split(‘, ’));
//rajoute un espace et une virgule entre chaque mot de l’array 

Pour faire un array : 

const numbers = new Array [1, 2, 3];
ou 
const fruits = [“apple”, “oranges”, 10];
console.log (fruits);

fruits [3] = ‘grapes’;
fruits.push(‘mangos’); // add
fruits.unshift(‘strawberries’); // enlever
fruits.pop(); 
console.log(fruits); //
console.log(fruits.indexOf(‘oranges’)); //donne la position du fruits dans la liste
——————————
const person = {
 firstName: ‘John’,
lastName: ‘Doe’,
hobbies: [music, dance, fuck],
address: {
	street: ‘234 rue des pyrénées’,
	city: ‘Paris’,
	}
}

console.log(person.hobbies[1]),

const {firstName, lastName, address: { city}} = person;

console.log (city);

————————————————

double guillemets en JSON alors qu’en Js on peut utiliser juste un guillemet 

——————————————-


For loop
for(let i = 0; i <= 10; i++) {
	console.log(‘For Loop Numer: ${i}’};
}

While loop
let i = 0;
while (i < 10) {
	console.log(‘While Loop Number: ${i}););
	i++;    //nécessaire pour  incrémenter
}

———————————

const todos = [
	{
		id: 3, 
		text: ‘Dentist appt’,
		isCompleted: false
	}

];

// forEach, map, filter 
`todos.forEach(function(todo) {
	console.log(todo.text);
});

const todoCompleted = todos.filter(function(todo) {
	return todo.iCompleted === true;
}).map(function(todo) {
	return todo.text;
});

——————————

simple condition 
&& II 

comple condition
const x = 10;

//? = then 
`const color = x > 20 ? ‘red’ : ‘blue;

switch(color) {
 case’red’:
	console.log(‘color is red’);
	break;
case’blue’ :
	console.log(‘color is blue’);
	break;
default:
	console.log(‘color is NOT red or blue’);
	break;
}`

——————————————

`function addNums(num1 = 1, num2 = 1) {
	return num1 + num2;
}

console.log(addNums(5, 5));`

——————————————

const addNums = num1 => num1 + 5;

console.log (addNums(5));
todos.forEach((todo));

_______________________

OBJECT ORIENTED PROGRAMMING

——————————————

//constructor function 
`function Person (first?ame, last?ame, dob) {
	this.firstName = firstName;
	this.lastName = lastName;
	this.dob = new Date(dob);
	this.getBirthYear = function() {
		return this.dob.getFullYear(); 
	}
	this.getFullName = function() {
		return ‘${this.firstName} ${this.lastName}`; }
}`

//instantiate object 
const person1 = new Person ((John, ‘Doe, ‘4-3-1980’);
const person2 = new Person (‘Mary’, ‘Jane’, ‘3-4-1993’);

console.log(person2.dob.getFullYear();
// 1980
console.log(person1.getFullName()};
// John Doe


****30 days challenge has started

**Day 1 done 

**Day 2 data type 

***In JavaScript the Math Object provides a lots of methods to work with numbers.

`
const PI = Math.PI

console.log(PI)                            // 3.141592653589793

// Rounding to the closest number
// if above .5 up if less 0.5 down rounding

console.log(Math.round(PI))                // 3 to round values to the nearest number

console.log(Math.round(9.81))              // 10

console.log(Math.floor(PI))                // 3 rounding down

console.log(Math.ceil(PI))                 // 4 rounding up

console.log(Math.min(-5, 3, 20, 4, 5, 10)) // -5, returns the minimum value

console.log(Math.max(-5, 3, 20, 4, 5, 10)) // 20, returns the maximum value

const randNum = Math.random() // creates random number between 0 to 0.999999
console.log(randNum)

// Let us  create random number between 0 to 10

const num = Math.floor(Math.random () * 11) // creates random number between 0 and 10
console.log(num)

//Absolute value
console.log(Math.abs(-10))      // 10

//Square root
console.log(Math.sqrt(100))     // 10

console.log(Math.sqrt(2))       // 1.4142135623730951

// Power
console.log(Math.pow(3, 2))     // 9

console.log(Math.E)             // 2.718

// Logarithm
// Returns the natural logarithm with base E of x, Math.log(x)
console.log(Math.log(2))        // 0.6931471805599453
console.log(Math.log(10))       // 2.302585092994046

// Trigonometry
Math.sin(0)
Math.sin(60)

Math.cos(0)
Math.cos(60)`


***- Long Literal Strings
We can use the backslash character (\) at the end of each line to indicate that the string will continue on the next line. Example:

const paragraph = "My name is Asabeneh Yetayeh. I live in Finland, Helsinki.\
I am a teacher and I love teaching. I teach HTML, CSS, JavaScript, React, Redux, \
Node.js, Python, Data Analysis and D3.js for anyone who is interested to learn. \
In the end of 2019, I was thinking to expand my teaching and to reach \
to global audience and I started a Python challenge from November 20 - December 19.\
It was one of the most rewarding and inspiring experience.\
Now, we are in 2020. I am enjoying preparing the 30DaysOfJavaScript challenge and \
I hope you are enjoying too."

console.log(paragraph)

***- Let's see the most common escape characters:

\n: new line
\t: Tab, means spaces
\\: Back slash
\': Single quote (')
\": Double quote (")

***Using a string template or string interpolation method, we can add expressions, which could be a value, or some operations (comparison, arithmetic operations, ternary operation).
`
let a = 2
let b = 3
console.log(`${a} is greater than ${b}: ${a > b}`)
2 is greater than 3: false`


***String Methods

toUppercase() / toLowerCase()
`
let string = 'JavaScript'
console.log(string.toUpperCase())     // JAVASCRIPT`

substr(): It takes two arguments, the starting index and number of characters to slice.
`
let string = 'JavaScript'
console.log(string.substr(4,6))    // Script`

split(): The split method splits a string at a specified place.
`
let string = '30 Days Of JavaScript'
console.log(string.split())     // Changes to an array -> ["30 Days Of JavaScript"]
console.log(string.split(' '))  // Split to an array at space -> ["30", "Days", "Of", "JavaScript"]`

trim(): Removes trailing space in the beginning or the end of a string.
`
let string = '   30 Days Of JavaScript   '
console.log(string)
console.log(string.trim(' '))
//    30 Days Of JavasCript   
//30 Days Of JavasCript
`

includes(),
replace(), 
charAt() : takes index and it returns the value at the index
`
let string = '30 Days Of JavaScript'
console.log(string.charAt(0))        // 3`

concat(),
startsWith(),
endsWith(),
search(),
`
let string = 'I love JavaScript. If you do not love JavaScript what else can you love.'
console.log(string.search('love'))          // 2
console.log(string.search(/javascript/gi))  // 7`

match(),
repeat()

**Checking data types and casting

 with typeof method : 
`
let firstName = 'Asabeneh'      // string
console.log(typeof 'Asabeneh')  // string
`

 Casting: Converting one data type to another data type. 
We use :

parseInt(), 
parseFloat(),
Number(), 
+ sign, 
+ str() 

     String to Int (parseInt(), Number(), Plus sign(+)) 
`
let num = '10'
let numInt = parseInt(num)
console.log(numInt) // 10

let num = '10'
let numInt = Number(num)
console.log(numInt) // 10

let num = '10'
let numInt = +num

console.log(numInt) // 10
`
    String to Float (parseFloat(), Number(), Plus sign(+))
    
`
let num = '9.81'
let numFloat = parseFloat(num)

console.log(numFloat) // 9.81
`



