# Day 5 

## Arrays
### Modifying array element
````
const countries = [
  'Albania',
  'Bolivia',
  'Canada',
  'Denmark',
  'Ethiopia',
  'Finland',
  'Germany',
  'Hungary',
  'Ireland',
  'Japan',
  'Kenya'
]

countries[0] = 'Afghanistan'  // Replacing Albania by Afghanistan
let lastIndex = countries.length - 1
countries[lastIndex] = 'Korea' // Replacing Kenya by Korea

console.log(countries)
````

### Methods to manipulate array

#### Array Constructor 
Array:To create an array.
````
const arr = Array() // creates an an empty array
console.log(arr)

const eightEmptyValues = Array(8) // it creates eight empty values
console.log(eightEmptyValues) // [empty x 8]
````
### Creating static values with fill
fill: Fill all the array elements with a static value
````
const arr = Array() // creates an an empty array
console.log(arr)

const eightXvalues = Array(8).fill('X') // it creates eight element values filled with 'X'
console.log(eightXvalues) // ['X', 'X','X','X','X','X','X','X']
````

### Concatenating array using concat
concat:To concatenate two arrays.
````
const firstList = [1, 2, 3]
const secondList = [4, 5, 6]
const thirdList = firstList.concat(secondList)

console.log(thirdList) // [1, 2, 3, 4, 5, 6]
````

### Getting array length
````
const numbers = [1, 2, 3, 4, 5]
console.log(numbers.length) // -> 5 is the size of the array
````
### Getting index an element in arr array & last index of an element array is .lastIndexOf
````
const numbers = [1, 2, 3, 4, 5]
console.log(numbers.indexOf(5)) // -> 4
````

Check an element if it exist in an array.

***Check items in a list
````
// let us check if a banana exist in the array

const fruits = ['banana', 'orange', 'mango', 'lemon']
let index = fruits.indexOf('banana')  // 0

if(index != -1){
   console.log('This fruit does exist in the array')  
} else {
    console.log('This fruit does not exist in the array')
}
// This fruit does exist in the array

// we can use also ternary here
index != -1 ? console.log('This fruit does exist in the array'): console.log('This fruit does not exist in the array')

// let us check if a avocado exist in the array
let indexOfAvocado = fruits.indexOf('avocado')  // -1, if the element not found index is -1
if(indexOfAvocado!= -1){
   console.log('This fruit does exist in the array')  
} else {
    console.log('This fruit does not exist in the array')
}
// This fruit does not exist in the array
````
***includes:To check if an item exist in an array. If it exist it returns the true else it returns false.
````
const numbers = [1, 2, 3, 4, 5]

console.log(numbers.includes(5)) // true
console.log(numbers.includes(0)) // false
````

***Checking array
Array.isArray:To check if the data type is an array
````
const numbers = [1, 2, 3, 4, 5]
console.log(Array.isArray(numbers)) // true
````

***Converting array to string
toString:Converts array to string
````
const numbers = [1, 2, 3, 4, 5]
console.log(numbers.toString()) // 1,2,3,4,5
````

***Joining array elements 
````
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook']

console.log(names.join()) // Asabeneh,Mathias,Elias,Brook
console.log(names.join('')) //AsabenehMathiasEliasBrook
console.log(names.join(' ')) //Asabeneh Mathias Elias Brook
````

***Slice array elements

Slice: To cut out a multiple items in range. It takes two parameters:starting and ending position. It doesn't include the ending position.
```
  const numbers = [1,2,3,4,5]

  console.log(numbers.slice()) // -> it copies all  item
  console.log(numbers.slice(0)) // -> it copies all  item
  console.log(numbers.slice(0, numbers.length)) // it copies all  item
  console.log(numbers.slice(1,4)) // -> [2,3,4] // it doesn't include the ending position
  ````

***Splice method in array

Splice: It takes three parameters:Starting position, number of times to be removed and number of items to be added.
````
  const numbers = [1, 2, 3, 4, 5]

  console.log(numbers.splice())                // -> remove all items
  const numbers = [1, 2, 3, 4, 5]
  console.log(numbers.splice(0,1))            // remove the first item
  const numbers = [1, 2, 3, 4, 5, 6];
  console.log(numbers.splice(3, 3, 7, 8, 9))  // -> [1, 2, 3, 7, 8, 9] //it removes three item and replace three items
  ````

***Add with push
````
const numbers = [1, 2, 3, 4, 5]
numbers.push(6)

console.log(numbers) // -> [1,2,3,4,5,6]

numbers.pop() // -> remove one item from the end
console.log(numbers) // -> [1,2,3,4,5]
````

***Removing the end element using pop

pop: Removing item in the end.
````
const numbers = [1, 2, 3, 4, 5]
numbers.pop() // -> remove one item from the end

console.log(numbers) // -> [1,2,3,4]
````

***Removing an element from the beginning

shift: Removing one array element in the beginning of the array.
````
const numbers = [1, 2, 3, 4, 5]
numbers.shift() // -> remove one item from the beginning

console.log(numbers) // -> [2,3,4,5]
````

***Add an element from the beginning

unshift: Adding array element in the beginning of the array.
````
const numbers = [1, 2, 3, 4, 5]
numbers.unshift(0) // -> add one item from the beginning

console.log(numbers) // -> [0,1,2,3,4,5]
````

