
Fundamentals
==================

## Data Types

- String
- Number
- Boolean

- undefined
- null

- symbol
- Bigint

- Array
- Object

<br />

_`typeof`  check the data type_

<br />




------

## Statements & expressions




### Expression examples
_expressions evaluates to a value_
```
1 + 1

'Hello' + ' ' + 'World'

```

### Statement examples 
_statements performs an action_

```
1 + 1 /// also a statement

if (i > 50) {
    return i
}

let greeting = "hello"

for(let i = 0; i < 50; i++) {
    console.log(i)
}

```
------
## Variables

- `var` (depricated)

- `let`

- `const`

### `let` examples

_block scope_


```
let greeting = "hello" // initial assignment

greeting = "hi" // okay to reassign

let greeting = "hey" // ERROR


```

### `const` examples
_constant referance to a value_
<br />
_cannot reassign the type but can change properties of objects and elements of arrays_
<br />
_block scope_

```
const PI = 3.14 // initial assignment

PI = 7 // ERROR

PI = PI + 100 // ERROR
```
```
const cats = ['bob', 'jeff', 'jane'] // initial assignment for array

cats.push('garfield') // adding/removing/changing elements to a constant array is fine

cats = ['scooby-doo', 'snoopy'] // cannot reassign the array // ERROR
```
```
// same concept as arrays with objects
const cat = {name: 'Garfield', age: 2, favFood: 'lasagna' }

cat.age = 5 // changing the property is okay

const cat = {name: 'scooby-doo', age: 100, favFood: 'scoobySnacks'} // ERROR // cannot reassign the object

```
---
## Operators 

### Arithmetic

|Operator|Meaning|
|:---:|:---| 
|+ |Addition
|-  |	Subtraction
|*  |	Multiplication
|** |	Exponentiation (ES2016)
|/  |    Division
|%  | 	Modulus (Division Remainder)
|++ |    Increment
|-- |	Decrement

---
### Assignment

|Operator|Example|Same As|
|:---:|:---:|:---:|
|=|   x = y   |	x = y
|+=|   x += y  |	x = x + y
|-=|   x -= y  |	x = x - y
|*=|   x *= y  |	x = x * y
|/=|   x /= y  |	x = x / y
|%=|   x %= y  |	x = x % y
|**=|   x **= y |	x = x ** y


---
## Conditional Statements

- `if`
- `else`
- `else if`
- `switch`

`if` to execute a block of code if the statement is true

```
let bottles = 99

if (bottles === 99) {
    console.log('99 bottles of beer on the wall') 
}
```
_console.log() will print out to console_

`else` will execute if the initial condition is false

```
let bottles = 98

if (bottles === 99) {
    console.log('99 bottles of beer on the wall') 
} else {
    console.log('there is not 99 bottles of beer on the wall')
}
```
`else if` adds another condition will only run if the initial condition is false.

```
let bottles = 98

if (bottles === 99) {
    console.log('99 bottles of beer on the wall') 
} else if (bottles === 98) {
    console.log('98 bottles of beer on the wall')
} else {
    console.log('there is not 99 bottles of beer on the wall')
}

```


---
## Arrays
_data type_

```
                        0           1          2     // index position of items in the array
const sportsList = ['football', 'skiing', 'cricket'] // initialise array

sportsList[1] -> skiing // access array item using the index

sportsList[0] -> football // access array item using the index

sportsList.push('swimming') -> ['football', 'skiing', 'cricket', swimming''] // add item to the end of the array

sportsList.pop() -> ['football', 'skiing', 'cricket'] // remove last item from array

sportsList.shift() -> ['skiing', 'cricket'] // remove first item from the array

sportsList.unshift('basketball') -> ['basketball', 'skiing', 'cricket'] // add item to beggining of array


```
_there are more array methods than I have listed here_


## Loops
> A loop is a sequence of instructions that is continually repeated until a certain condition is met

```
for (statement 1; statement 2; statement 3){
    execute code block
}
```
```
Create variable i, check if i is less than 10, if less than 10 add 1 to i and execute code in block. repeat.
for(let i = 0; i < 10; i++){
    console.log(i)
} 

//This loop will print numbers 0-9, will stop when condition is met (i = 10)
```

_there are a few variations of for loop syntax in js ther are also while loops_


## Objects
_data type_

_key value pairs_

```
const person = {
    name: 'bob',
    age: 50,
}
// In this example 'name' is a key and 'bob' is a value

person.name -> bob // access the vairable
person['name'] -> bob // same just different syntax

person.name = 'john' // change the variable

person.hobbies = 'reading' // add another key value pair


```

## Functions

> Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

```
// define the function
function square(number) {
    return number * number;
}

// call the function, argument is 5, return value is 25
square(5) -> 25

// call the function, argument is 2, return value is 4
square(2) -> 4

```


> Quotes and code snippets used from [MDN](https://developer.mozilla.org/en-US/docs) and [W3schools](https://www.w3schools.com/)