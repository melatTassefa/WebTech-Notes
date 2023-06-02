# JavaScript Basic Concepts 5

# Arrays

An array is a collection of different data types which are ordered and changeable(modifiable). An array allows storing duplicate elements and different data types. An array can be empty, or it may have different data type values.

## How to create an empty array

- Using Array constructor

```jsx
// syntax
const arr = Array()// or// 
let arr = new Array()
console.log(arr)
```

- Using square brackets([])

```jsx
// syntax// This the most recommended way to create an empty list
const arr = []
console.log(arr)
```

## How to create an array with values

Array with initial values. We use *length* property to find the length of an array.

```jsx
const numbers = [0, 3.14, 9.81, 37, 98.6, 100]  // set of numbers
console.log(numbers.length)  // => to know the size of the array, which is 6
```

- Array can have items of different data types

```jsx
const arr = ['Ada', 4, 'Abe', 5, 'Ama', 4.5]
```

## Creating an array using split

Use the split method in the string object.

```jsx
let js = 'JavaScript, python, c++'
let js2 = js.split(,);
console.log(js2)  // ['JavaScript', 'python', 'c++']
```

## Accessing array items using index

We access each element in an array using their index. An array index starts from 0.

## Modifying array element

```jsx
const numbers = [1, 2, 3, 4, 5]
numbers[0] = 10  // the first element is changed to 10
```

## Methods to manipulate array

There are different methods to manipulate an array. These are some of the available methods to deal with arrays:*Array, length, concat, indexOf, slice, splice, join, toString, includes, lastIndexOf, isArray, fill, push, pop, shift, unshift.*

### Creating static values with fill

Fill all the array elements with a static value.

### Concatenating array using concat

To concatenate two arrays.

```jsx
const arr = Array();
arr(7).fill('d');  // fill the array with 7 ds
const arr2 = [1,2,3]
const arr3 = arr.concat(arr2)  //concatenate the two arrays

```

### Getting index of an element in an array

indexOf:To check if an item exist in an array. If it exists it returns the index else it returns -1.

### Getting last index of an element in array

lastIndexOf: It gives the position of the last item in the array. If it exist, it returns the index else it returns -1.

### Checking array

Array.isArray:To check if the data type is an array.

### Converting array to string

toString:Converts array to string

### Joining array elements

join: It is used to join the elements of the array, the argument we passed in the join method will be joined in the array and return as a string. By default, it joins with a comma, but we can pass different string parameter which can be joined between the items.

```jsx
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook']
console.log(names.join(' ')) //Asabeneh Mathias Elias Brook
```

### Slice array elements

Slice: To cut out a multiple items in range. It takes two parameters:starting and ending position. It doesn’t include the ending position.

### Splice method in array

Splice: It takes three parameters: Starting position, number of times to be removed and number of items to be added.

```jsx
const numbers = [1, 2, 3, 4, 5, 6]    
numbers.splice(3, 2, 7, 8, 9)  
console.log(numbers)  // -> [1, 2, 3, 7, 8, 9, 6] // it starts from 3 and it removes three items and replace three items
```

### Adding item to an array using push

Push: adding item in the end. To add item to the end of an existing array we use the push method.

### Removing the end element using pop

pop: Removing item in the end.

### Removing an element from the beginning

shift: Removing one array element in the beginning of the array.

### Add an element from the beginning

unshift: Adding array element in the beginning of the array.

### Reversing array order

reverse: reverse the order of an array.

### Sorting elements in array

sort: arrange array elements in ascending order. Sort takes a call back function, we will see how we use sort with a call back function in the coming sections.

### Array of arrays

Array can store different data types including an array itself.

```jsx
const firstNums = [1, 2, 3]
const secondNums = [1, 4, 9]const 
arrayOfArray =  [[1, 2, 3], [1, 2, 3]]
console.log(arrayOfArray[0]) // [1, 2, 3]
```