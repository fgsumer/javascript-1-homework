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
function copyMachine(arr, num) {
  let newArr = [];
  while (num >= 1) {
   
  newArr.push([...arr]); // we need to make it two times.
   
    num--;
  }
  return newArr;
}

// change code here to test different cases:
console.log(copyMachine([true, false, true], 2));
```
### Combine Arrays with the Spread Operator
```js
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence = ['learning', ...fragment,'is', 'fun']; 
  return sentence; // returns['learning', 'to', 'code', 'is', 'fun'].
}

// do not change code below this line
console.log(spreadOut());
```
### Check For The Presence of an Element With indexOf()
indexOf(), that allows us to quickly and easily check for the presence of an element on an array. indexOf() takes an element as a parameter, and when called, it returns the position, or index, of that element, or -1 if the element does not exist on the array.
```js
function quickCheck(arr, elem) {
  // change code below this line
  if (arr.indexOf(elem) === -1) {
    return false; 
  } else {
    return true;
  }
  // change code above this line
}

// change code here to test different cases:
console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));
```
### Iterate Through All an Array's Items Using For Loops
```js
function filteredArray(arr, elem) {
  let newArr = [];
  // change code below this line
for (let i = 0; i < arr.length; i++) {
   if (arr[i].indexOf(elem)===-1){
     newArr.push(arr[i]);
}
}
  // change code above this line
  return newArr;
}

// change code here to test different cases:
console.log(filteredArray([[3, 2, 3], [1, 6, 3], [3, 13, 26], [19, 3, 9]], 3));
```
### Create complex multi-dimensional arrays
```js
let myNestedArray = [
  // change code below this line
  ['unshift', false, 1],           //level 2
  [3, 'complex', 'nested', false], //level 2
  [
    ['mutate', 98, true, 'deep'], //level 3
    [
      ['splice', 7, false, 'deeper'], //level 4
      [
        ['iterate', 3849, 7, 'deepest'], //level 5
      ],
    ],
  ],
 ];
 
```
### Add Key-Value Pairs to JavaScript Objects
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
### 
```js

```
