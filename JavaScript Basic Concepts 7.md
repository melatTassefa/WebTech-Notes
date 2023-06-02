# JavaScript Basic Concepts 7

# Functions

A function is a reusable block of code or programming statements designed to perform a certain task. A function is declared by a function key word followed by a name, followed by parentheses ().

A function can be declared or created in the following ways:

- *Declaration function*
- *Expression function*
- *Anonymous function*
- *Arrow function*

## Function Declaration

```jsx
function square() { 
let num = 2  
let sq = num * num  
console.log(sq)}
square() // 4
```

## Function returning value

Function can also return values, if a function does not return values the value of the function is undefined.

```jsx
function printFullName (){
let firstName = 'Asabeneh'
let lastName = 'Yetayeh'
let space = ' '
let fullName = firstName + space + lastName      
return fullName}
console.log(printFullName())
```

## Function with a parameter

In a function we can pass different data types(number, string, boolean, object, function) as a parameter.

```jsx
function sumTwoNumbers(numOne, numTwo) {  
let sum = numOne + numTwo  
console.log(sum)}
sumTwoNumbers(10, 20)
```

### Unlimited number of parameters in regular function

```jsx
sumAllNums() {  
let sum = 0  
for (let i = 0; i < arguments.length; i++) {    
sum += arguments[i]  }  
return sum}
console.log(sumAllNums(1, 2, 3, 4)) // 10
console.log(sumAllNums(10, 20, 13, 40, 10))  // 93
```

### Unlimited number of parameters in arrow function

Arrow function does not have the function scoped arguments object. To implement a function which takes unlimited number of arguments in an arrow function we use spread operator(…) followed by any parameter name. Any thing we passed as argument in the function can be accessed as array in the arrow function. 

## Anonymous Function

Anonymous function or without name.

```jsx
const anonymousFun = function() {  
console.log('I am an anonymous function and my value is stored in anonymousFun'  )}
```

## Expression Function

Expression functions are anonymous functions. After we create a function without a name and we assign it to a variable, to return a value from the function, we should call the variable.

```jsx
const square = function(n) { 
return n * n}
console.log(square(2)) // -> 4
```

## Self Invoking Functions

Self invoking functions are anonymous functions which do not need to be called to return a value.

```jsx
let squaredNum = (function(n) {  return n * n})(10)
console.log(squaredNum)  //100
```

## Arrow Function

Arrow function uses arrow instead of the keyword *function* to declare a function.

```jsx
square = n => {  return n * n}
console.log(square(2))
```

## Function with default parameters

Sometimes we pass default values to parameters, when we invoke the function if we do not pass an argument the default value will be used. Both function declaration and arrow function can have a default value or values.

```jsx
function greetings(name = 'Peter') {  
let message = `${name}, welcome to 30 Days Of JavaScript!`  
return message}
console.log(greetings()) // Peter, welcome to 30 Days Of JavaScript!
console.log(greetings('Asabeneh')) // Asabeneh, welcome to 30 Days Of JavaScript!
```