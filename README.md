# Coding-diary
Everyday learning

Friday 2nd of April

Have to redo all my work there is something wrong with the css
it doesn't adds on. 

Monday 5th of April 

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



