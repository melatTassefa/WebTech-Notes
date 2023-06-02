# JavaScript Basic Concepts 6

# Loops

Different kinds of loops are used to carry out a repetitive task.

## For Loop

```jsx
const arr = [1,2,3,4]
for( let i=0;i<arr.length;i++){
	console.log(arr[i]);
}

```

Creating a new array based on the existing array

```jsx
const numbers = [1, 2, 3, 4, 5]
const newArr = []
let sum = 0
for(let i = 0; i < numbers.length; i++){  
newArr.push( numbers[i] ** 2)}
console.log(newArr)  // [1, 4, 9, 16, 25]
```

## While Loop

```jsx
const arr = [1,2,3,4]
let i = 0;
while (i < arr.length){
console.log(arr[i]);
}
```

## do while Loop

```jsx
let i = 0
do {  console.log(i)  i++} 
while (i <= 5)// 0 1 2 3 4 5
```

## for of Loop

```jsx
const numbers = [1, 2, 3, 4, 5]
for (const num of numbers) {  
console.log(num)}// 1 2 3 4 5
```

## Break

Break is used to interrupt a loop.

```jsx
for(let i = 0; i <= 5; i++){  
if(i == 3){   
break} 
 console.log(i)}// 0 1 2
```

## Continue

We use the keyword *continue* to skip a certain iterations.

```jsx
for(let i = 0; i <= 5; i++){  
if(i == 3){
continue}
console.log(i)}// 0 1 2 4 5
```