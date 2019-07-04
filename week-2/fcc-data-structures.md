> begin [the basic data structure exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-data-structures) and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  

### Use an Array to Store a Collection of Data
```js
let yourArray = ["yogurt", 5, false, true, "tea"]; 
```
### Access an Array's Contents Using Bracket Notation
```js
let myArray = ["a", "b", "c", "d"];
// change code below this line

myArray[1] = "kitten";
```
### Add Items to an Array with push() and unshift()
the push() method adds elements to the end of an array, and unshift() adds elements to the beginning. 
```js
function mixedNumbers(arr) {
 
arr.unshift('I', 2, 'three');
arr.push(7, 'VIII', 9);

  return arr;
}

// do not change code below this line
console.log(mixedNumbers(['IV', 5, 'six']));

```
### Remove Items from an Array with pop() and shift()
pop() removes an element from the end of an array, while shift() removes an element from the beginning. 

```js
function popShift(arr) {
  let popped = arr.pop(); // change this line
  let shifted = arr.shift(); // change this line
  return [shifted, popped];
}

// do not change code below this line
console.log(popShift(['challenge', 'is', 'not', 'complete']));
```
### Remove Items Using splice()
splice() allows us to do just that: remove any number of consecutive elements from anywhere in an array. splice()'s first parameter represents the index on the array from which to begin removing elements, while the second parameter indicates the number of elements to delete. 

```js 
function sumOfTen(arr) {   //Modify the function, using splice(), so that it returns a value of 10.
  // change code below this line
  let reduce = arr.splice(1, 2);
  // change code above this line
  return arr.reduce((a, b) => a + b);
}

// do not change code below this line
console.log(sumOfTen([2, 5, 1, 5, 2, 1]));

```
### Add Items Using "splice()"
```js
function htmlColorNames(arr) {
  // change code below this line
  arr.splice(0, 2, "DarkSalmon", "BlanchedAlmond");
  
  // change code above this line
  return arr;
} 
 
// do not change code below this line
console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurqoise', 'FireBrick'])); 

// result is DarkSalmon,BlanchedAlmond,LavenderBlush,PaleTurqoise,FireBrick

```
### Copy Array Items Using "slice()"
rather than modifying an array, copies, or extracts, a given number of elements to a new array, leaving the array it is called upon untouched. 
```js
function forecast(arr) {
 

  return arr = arr.slice(2, 4);  // warm,sunny
}

// do not change code below this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms'])); 

```
### Copy an Array with the Spread Operator 
```js

```
### 
```js

```
### 
```js

```
### 
```js

```
### 
```js

```
### 
```js

```
### 
```js

```
### Last loop value
```js

```
### Last loop value
```js

```
### Last loop value
```js

```
### Last loop value
```js

```
### Last loop value
```js

```
### Last loop value
```js

```
