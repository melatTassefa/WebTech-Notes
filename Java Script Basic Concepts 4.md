# Java Script Basic Concepts 4

# Conditionals

Conditional statements are used to make decisions based on different conditions. If the processing logic require so, the sequential flow of execution can be altered in two ways:

- Conditional execution: a block of one or more statements will be executed if a certain expression is true
- Repetitive execution: a block of one or more statements will be repetitively executed as long as a certain expression is true. In this section, we will cover *if*, *else* , *else if* statements. The comparison and logical operators we learned in the previous sections will be useful in here.

Conditions can be implementing using the following ways:

- if
- if else
- if else if else
- switch
- ternary operator

## If

It is to used check if a condition is true and to execute the block code.

```jsx
let num = 5
if (num > 0) {  
console.log(`${num} is a positive number`)}//  5 is a positive number
```

## If Else

If condition is true the first block will be executed, if not the else condition will be executed.

```jsx
let num = -5
if (num > 0) {  console.log(`${num} is a positive number`)}
else {  console.log(`${num} is a negative number`)}//  -5 is a negative number
```

## If Else if Else

We use else if when we have multiple conditions.

```jsx
let a = 0
if (a > 0) {  console.log(`${a} is a positive number`)} 
else if (a < 0) {  console.log(`${a} is a negative number`)} 
else if (a == 0) {  console.log(`${a} is zero`)} 
else {  console.log(`${a} is not a number`)}
```

## Switch

Switch works similar to if else if else. The variable in the parenthesis is checked and if it matches the value of the cases, the code in that block is executed. The break statement is to terminate execution so the code execution does not go down after the condition is satisfied. The default block runs if all the cases don’t satisfy the condition.

```jsx
let str = 'Hello'
let num = str.length;
switch(num){
  case 0:
    console.log("Empty");
  case 1:
    console.log("1 letter");
  case 2:
    console.log("2 letters");
  default:
    console.log("Too many letters");
}
```

## Ternary Operators

Syntax
Condition ? Execute if Condition is true : Execute if Condition is false

```jsx
let isRaining = true
isRaining  ? console.log('You need a rain coat.')  : console.log('No need for a rain coat.')
```