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
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28
};

// change code below this line
foods.bananas = 13;
foods.grapes = 35;
foods.strawberries= 27;
// change code above this line

console.log(foods);
```
### Modify an Object Nested Within an Object
```js
let userActivity = {
  id: 23894201352,
  date: 'January 1, 2017',
  data: {
    totalUsers: 51,
    online: 42
  }
};

// change code below this line
userActivity.data.online = 45;
// change code above this line

console.log(userActivity);
```
### Access Property Names with Bracket Notation
```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};
function checkInventory(scannedItem) {
  return foods[scannedItem];
}
console.log(checkInventory("apples"));
```
### Use the delete Keyword to Remove Object Properties
```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};

delete foods.oranges;
delete foods.plums;
delete foods.strawberries;


console.log(foods);
```
### Check if an Object has a Property
if we want to know if an object has a specific property, we can do it in two different ways : "hasOwnProperty()" method or "in" keyword.
```js
let users = {
   Alan: {
    age: 27,
    online: true
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: true
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function isEveryoneHere(obj) {
  // change code below this line
if (obj.hasOwnProperty("Alan", "Jeff", "Sarah", "Ryan")){
  return true;
} else {
  return false;
}
  // change code above this line
}

console.log(isEveryoneHere(users));
```
### Iterate Through the Keys of an Object with a for...in Statement
```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function countOnline(obj) {
  
  let userNumber = 0;
	for (let user in obj) if (obj[user].online) userNumber++;
	return userNumber;
};

console.log(countOnline(users));
```
### Generate an Array of All Object Keys with Object.keys()
We can  generate an array which contains all the keys stored in an object using the Object.keys() method and passing in an object as the argument. This will return an array with strings representing each property in the object. 
```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function getArrayOfUsers(obj) {
return Object.keys(obj);
}

console.log(getArrayOfUsers(users));
```
### Modify an Array Stored in an Object
```js
let user = {
  name: 'Kenneth',
  age: 28,
  data: {
    username: 'kennethCodesAllDay',
    joinDate: 'March 26, 2016',
    organization: 'freeCodeCamp',
    friends: [
      'Sam',
      'Kira',
      'Tomo'
    ],
    location: {
      city: 'San Francisco',
      state: 'CA',
      country: 'USA'
    }
  }
};

function addFriend(userObj, friend) {
 
  userObj.data.friends.push(friend);
  return userObj.data.friends;

}
console.log(addFriend(user, 'Pete'));
```


