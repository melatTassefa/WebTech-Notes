# JavaScript Basic Concepts 8

# Objects

## Scope

A variable can be declared at different scope. They are:

- Global
- Local

### Window Global Object

```jsx
a = 'JavaScript' // declaring a variable without let or const makes it available in window object and it's found anywhere
```

### Global scope

A globally declared variable can be accessed every where in the same file. But the term global is relative. It can be global to the file or it can be global relative to some block of codes.

### Local scope

A variable declared as local can be accessed only in certain block code.

- Block Scope
- Function Scope

A variable declared with *var* only scoped to function but variable declared with *let* or *const* is block scope(function block, if block, loop block, etc). Block in JavaScript is a code in between two curly brackets ({}).

## Object

Objects do have properties and properties have values, so an object is a key value pair. The order of the key is not reserved, or there is no order. To create an object literal, we use two curly brackets.

### Creating an empty object

```jsx
const person = {}
```

### Creating an object with values

```jsx
const rectangle = {  length: 20,  width: 20}
console.log(rectangle) // {length: 20, width: 20}
```

### Getting values from an object

We can access values of object using two methods:

- using . followed by key name if the key-name is a one word
- using square bracket and a quote

```jsx
const person = {  firstName: 'Asabeneh',  lastName: 'Yetayeh',  age: 250
getFullName: function() {    return `${this.firstName}${this.lastName}`  }}
console.log(person.firstName)
console.log(person['age'])
```

### Creating object methods

A function inside an object is called object method. The *this* key word refers to the object itself. We can use the word *this* to access the values of different properties of the object.

### Object Methods

- *Object.assign*: To copy an object without modifying the original object.
- *Object.keys*: To get the keys or properties of an object as an array
- *Object.values*:To get values of an object as an array
- *Object.entries*:To get the keys and values in an array
- *hasOwnProperty*: To check if a specific key or property exist in an object