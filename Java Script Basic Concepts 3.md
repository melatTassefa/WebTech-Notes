# Java Script Basic Concepts 3

# Booleans, Operators, Date

## Booleans

Boolean value is either true or false.

### Truthy values

- All numbers(positive and negative) are truthy except zero
- All strings are truthy except an empty string (’’)
- The boolean true

### Falsy values

- 0
- 0n
- null
- undefined
- NaN
- the boolean false
- ’’, "", ``, empty string

### Undefined

If we declare a variable and if we do not assign a value, the value will be undefined. In addition to this, if a function is not returning the value, it will be undefined.

## Operators

### Assignment operators(=)

They are used to assign a variable.

### Arithmetic Operators(+, -, *, /, %, **)

They are mathematical operators.

### Comparison Operators(>, <, ==, ===, <=, >=, !==, !=)

- ==(compares only value)
- ===(compares value and data types)
- !==(Negation of ===)
- !=(Negation of ==)

```jsx
console.log(3 != '3') //false
console.log(3 == '3') //true
console.log(3 ==='3') //false
```

As rule of thumb, if a value is not true with == it will not be equal with ===. Using === is safer than using ==.

### Increment Operator(++)

It is used to increase a value stored in a variable.

- Pre-increment: uses the principle, "Increase then Use”
- Post-increment: uses the principle, "Use then Increase”

```jsx
let x = 1, y = 3;
console.log(++x); // 2
console.log(y++); // 3
console.log(y); // 4
```

### Decrement Operator(—)

It is used to decrease a value stored in a variable.

- Pre-decrement: uses the principle, "decrease then Use”
- Post-decrement: uses the principle, "Use then decrease”

```jsx
let x = 1, y = 3;
console.log(--x); // 0
console.log(y--); // 3
console.log(y); // 2
```

### Ternary Operators(? : )

They allow to write a condition.

```jsx
let isRaining = true;
isRaining  ? console.log('You need a rain coat.')  : console.log('No need for a rain coat.')  //You need a rain coat
```

### Operator Precedence

Operator precedence determines how operators are parsed concerning each other. Operators with higher precedence become the operands of operators with lower precedence.

## Window Methods

### Window alert() method

alert() method displays an alert box with a specified message and an OK button. It is a builtin method and it takes on argument.

```jsx
alert(Alert!)
```

### Window prompt() method

It displays a prompt box with an input on your browser to take input values and the input data can be stored in a variable. The prompt() method takes two arguments. The second argument is optional.

### Window confirm() method

It displays a dialog box with a specified message, along with an OK and a Cancel button. A confirm box is often used to ask permission from a user to execute something. Window confirm() takes a string as an argument. Clicking the OK yields true value, whereas clicking the Cancel button yields false value.

```jsx
const agree = confirm('Are you sure you like to delete? ')
console.log(agree) // result will be true or false based on what you click on the dialog box
```

## Date Object

The object we create using Date object provides many methods to work with date and time. getFullYear(), getMonth(), getDate(), getDay(), getHours(), getMinutes, getSeconds(), getMilliseconds(), getTime(), getDay() are some of the methods.

```jsx
const now = new Date()
console.log(now.getFullYear()) // 2020
console.log(now.getMonth())   //5, June

```

### Getting time

This method gives time in milliseconds starting from January 1, 1970. It is also know as Unix time.

```jsx
const now = new Date() 
console.log(now.getTime()) // 1578092201341, this is the number of seconds passed from January 1, 1970 to January 4, 2020 00:56:41
```

```jsx
const allSeconds = Date.now() 
console.log(allSeconds) // 1578092201341, this is the number of seconds passed from January 1, 1970 to January 4, 2020 00:56:41
const timeInSeconds = new Date().getTime()
console.log(allSeconds == timeInSeconds) // true
```