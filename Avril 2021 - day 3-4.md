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
The following symbols are the common logical operators: 
&&(ampersand) , ||(pipe) and !(negation). 
The && operator gets true only if the two operands are true. The || operator gets true either of the operand is true. The ! operator negates true to false and false to true.
```

// && ampersand operator example const check = 4 > 3 && 10 > 5 // true && true -> true const check = 4 > 3 && 10 < 5 // true && false -> false const check = 4 < 3 && 10 < 5 // false && false -> false

// || pipe or operator, example const check = 4 > 3 || 10 > 5 // true || true -> true const check = 4 > 3 || 10 < 5 // true || false -> true const check = 4 < 3 || 10 < 5 // false || false -> false

//! Negation examples let check = 4 > 3 // true let check = !(4 > 3) // false let isLightOn = true let isLightOff = !isLightOn // false let isMarried = !false // true
```


### Increment Operators & Decrement avec -- pareil
```

Pre-increment 
let count = 0 
console.log(++count) // 1 
console.log(count) // 1 

Post-increment
let count = 0 console.log(count++) // 0 
console.log(count) // 1
```

### Ternary Operators
```

let isRaining = true isRaining 
? console.log('You need a rain coat.') 
: console.log('No need for a rain coat.') 
isRaining = false

isRaining 
? console.log('You need a rain coat.') 
: console.log('No need for a rain coat.') 

You need a rain coat. 
No need for a rain coat.
```

## Window Methods

prompt(),
confirm(),

# Data Object
## Time Object 

````
const now = new Date()
console.log(now) // Sat Jan 04 2020 00:56:41 GMT+0200 (Eastern European Standard Time)
console.log(now.getFullYear());

//lets make it readable
const now = new Date()
const year = now.getFullYear() // return year
const month = now.getMonth() + 1 // return month(0 - 11)
const date = now.getDate() // return date (1 - 31)
const hours = now.getHours() // return number (0 - 23)
const minutes = now.getMinutes() // return number (0 -59)

console.log(`${date}/${month}/${year} ${hours}:${minutes}`) // 4/1/2020 0:56

//GETTING TIME
const now = new Date() //
console.log(now.getTime()) // 1578092201341, this is the number of seconds passed from January 1, 1970 to January 4, 2020 00:56:41
````




[Image](src:https://github.com/Asabeneh/30-Days-Of-JavaScript/blob/master/images/date_time_object.png)





