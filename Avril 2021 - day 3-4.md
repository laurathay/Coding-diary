# Booleans

## Get date
getFullYear() : 2020
getMonth() : 0- 11
getDate() : day as number 0 - 31
getHours() :
getMinutes() :
getSeconds() : milliseconde
getTime() : milliseconde 
getDay() : weekday 0-6

## Comparison Operators
The following symbols are the common logical operators: &&(ampersand) , ||(pipe) and !(negation). The && operator gets true only if the two operands are true. The || operator gets true either of the operand is true. The ! operator negates true to false and false to true.

// && ampersand operator example
const check = 4 > 3 && 10 > 5         // true && true -> true
const check = 4 > 3 && 10 < 5         // true && false -> false
const check = 4 < 3 && 10 < 5         // false && false -> false

// || pipe or operator, example
const check = 4 > 3 || 10 > 5         // true  || true -> true
const check = 4 > 3 || 10 < 5         // true  || false -> true
const check = 4 < 3 || 10 < 5         // false || false -> false

//! Negation examples
let check = 4 > 3                     // true
let check = !(4 > 3)                  //  false
let isLightOn = true
let isLightOff = !isLightOn           // false
let isMarried = !false                // true



## Increment Operators & Decrement avec -- pareil

Pre-increment
let count = 0
console.log(++count)        // 1
console.log(count)          // 1
Post-increment
let count = 0
console.log(count++)        // 0
console.log(count)          // 1

##Ternary Operators 

let isRaining = true
isRaining
  ? console.log('You need a rain coat.')
  : console.log('No need for a rain coat.')
isRaining = false

isRaining
  ? console.log('You need a rain coat.')
  : console.log('No need for a rain coat.')
You need a rain coat.
No need for a rain coat.


