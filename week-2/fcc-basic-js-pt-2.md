> complete the rest of [basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) on FCC and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 

## 1. Selecting from Many Options with Switch Statements

f you have many options to choose from, use a **switch** statement. A switch statement tests a value and can have many case statements which define various possible values. Statements are executed from the first matched case value until a **break** is encountered.
```js
function caseInSwitch(val) {
  var answer = "";
  
  switch (val) {
    case 1:
    return "alpha";
    break;

    case 2:
    return "beta"; 
    break;
    
    case 3:
    return "gamma";
    break;
    case 4: 
    return "delta";
    break;
  }
  
  return answer;  
}

caseInSwitch(1);
```

## 2. Adding a Default Option in Switch Statements
```js
function switchOfStuff(val) {
  var answer = "";

 switch (val) {
   case "a":
   return "apple";
   break;

   case "b":
   return "bird";
   break;

   case "c":
   return "cat";
   break;

  default:
  return "stuff"
 }
  
  return answer;  
}
switchOfStuff(1);
```

## 3.Multiple Identical Options in Switch Statements
If the **break** statement is omitted from a switch statement's case, the following case statement(s) are executed until a break is encountered. If you have multiple inputs with the same output, you can use break after these many statements.

```
function sequentialSizes(val) {
  var answer = "";
 
  switch (val) {
    case 1:
    case 2:
    case 3:
    return "Low";
    break;

    case 4:
    case 5:
    case 6:
    return "Mid";
    break;

    case 7:
    case 8:
    case 9:
    return "High";
    break;
  }
  
  return answer;  
}
sequentialSizes(1);

```

## 4. Replacing If Else Chains with Switch

#### From if statement 
```js

function chainToSwitch(val) {
  var answer = "";
  // Only change code below this line
  
  if (val === "bob") {
    answer = "Marley";
  } else if (val === 42) {
    answer = "The Answer";
  } else if (val === 1) {
    answer = "There is no #1";
  } else if (val === 99) {
    answer = "Missed me by this much!";
  } else if (val === 7) {
    answer = "Ate Nine";
  }
  return answer;  
}

chainToSwitch(7);
```
#### to switch statement
```js
function chainToSwitch(val) {
  var answer = "";
  
  switch (val) {
    case "bob": 
    return "Marley";
    break;

    case 42:
    return "The Answer";
    break;

    case 1:
    return "There is no #1";
    break;

    case 99:
    return "Missed me by this much!"
    break; 

    case 7:
    return "Ate Nine";
  }
 
  return answer;  
}
chainToSwitch(7);
```

## 5. Returning Boolean Values from Functions
Instead of if statement for comparision, you can use another way below.
```js
function isLess(a, b) {
  if (a < b) {
    return true;
  } else {
    return false;
  }
}
isLess(10, 15);


function isLess(a, b) {
  return a <= b;
}
isLess(15, 10);

```
## 6. Return Early Pattern for Functions

```js
 
function abTest(a, b) {
 
  if (a < 0 || b < 0) {
      return undefined;
      } else {
      
  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}
}
// Change values below to test your code

abTest(2,2);
  
```

## 7.Counting Cards
```js
var count = 0;

function cc(card) {
  // Only change code below this line
  switch (card) {
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      count++;
    break; 
    case 7:
    case 8:
    case 9:
      count;
      break;
  case 10:
  case 'J':
  case 'Q':
  case 'K':
  case 'A':
    count--;
    break;

  }
  if (count > 0) {
    return count + " Bet"
  } else {
    return count + " Hold"
  }
  // Only change code above this line
}

```
## 8. Build JavaScript Objects
objects and their properties 
```js
var myDog = {
  "name" : "Zoe",
  "legs" : 4,
  "tails" : 1,
  "friends" : ["balls", "bones"]
};
```
## 9. Accessing Object Properties with Dot Notation
There are two ways to access the properties of an object: **dot notation (.)** and **bracket notation ([]),** similar to an array. Dot notation is what you use when you know the name of the property you're trying to access ahead of time.
```js

var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

var hatValue = testObj.hat;      
var shirtValue = testObj.shirt;   
```
## 10. Accessing Object Properties with Bracket Notation
```js
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

var entreeValue = testObj["an entree"]; 
var drinkValue = testObj["the drink"]; 
```
## 11. Accessing Object Properties with Variables

```js
// Setup
var testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};

var playerNumber = 16;      
var player = testObj[playerNumber];

```

## 12. Updating Object Properties

```js
var myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

myDog.name = "Happy Coder";

```

## 13. Add New Properties to a JavaScript Object

You can add new properties to existing JavaScript objects the same way you would modify them.
```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

myDog.bark = "Wouf-Wouf";
```

## 14. Delete Properties from a JavaScript Object
```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};
delete myDog.tails; 

```

## 15. Using Objects for Lookups
If you have tabular data, you can use an object to "lookup" values rather than a switch statement or an if/else chain. This is most useful when you know that your input data is limited to a certain range.

#### from  swıtch
```js
switch(val) {
    case "alpha": 
      result = "Adams";
      break;
    case "bravo": 
      result = "Boston";
      break;
    case "charlie": 
      result = "Chicago";
      break;
    case "delta": 
      result = "Denver";
      break;
    case "echo": 
      result = "Easy";
      break;
    case "foxtrot": 
      result = "Frank";
  }
  ```
  
  #### to objects
  
  ```js
  var lookup = {
  "alpha" : "Adams",
  "bravo" : "Boston",
  "charlie" : "Chicago",
  "delta" : "Denver",
  "echo" : "Easy", 
  "foxtrot" : "Frank"
  } ;
  
result = lookup[val];

```
## 16. Testing Objects for Properties
```js

var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {
  if (myObj.hasOwnProperty(checkProp) == true) {
    return myObj[checkProp];
  } else {
    return "Not Found"
  }
}
```
## 17. Manipulating Complex Objects
```js

```
## 18. Accessing Nested Objects

```js
var myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};

var gloveBoxContents = myStorage.car.inside[ "glove box" ];

```
## 19. Accessing Nested Arrays
```js

var myPlants = [
  { 
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }  
];


var secondTree = myPlants[1].list[1]; // pine 
```
## 20. Record Collection (full sample)
```js
// Setup
var collection = {
    "2548": {
      "album": "Slippery When Wet",
      "artist": "Bon Jovi",
      "tracks": [ 
        "Let It Rock", 
        "You Give Love a Bad Name" 
      ]
    },
    "2468": {
      "album": "1999",
      "artist": "Prince",
      "tracks": [ 
        "1999", 
        "Little Red Corvette" 
      ]
    },
    "1245": {
      "artist": "Robert Palmer",
      "tracks": [ ]
    },
    "5439": {
      "album": "ABBA Gold"
    }
};
// Keep a copy of the collection for tests
var collectionCopy = JSON.parse(JSON.stringify(collection));

// Only change code below this line

function updateRecords(id, prop, value) {
  if (prop === "tracks" && value !== "") {
    if (collection[id][prop]) {
      collection[id][prop].push(value);
    }
    else {
      collection[id][prop] = [value];
    } 
  }
  else if (value !== "") {
      collection[id][prop] = value;
    }
    else {
      delete collection[id][prop];
    }
  
  return collection;
}

// Alter values below to test your code
updateRecords(5439, "artist", "ABBA");
```

## 21. Iterate with JavaScript While Loops

```js
var myArray = [];
var i = 0; 
while (i <= 4) {
    myArray.push(i);
    i++;
}

```

## 22. Iterate with JavaScript For Loops
```js

var myArray = [];
for (var i= 1; i <= 5; i++) {
    myArray.push(i)
}
```
## 23. Iterate Odd Numbers With a For Loop
```js
var myArray = [];

for (var i= 1; i <= 9; i += 2 )
{
  myArray.push(i);
}

```

## 24. Count Backwards With a For Loop

```js
var myArray = [];

for (var i = 9; i > 0; i -= 2) {
  myArray.push(i)
}

```

## 25. Iterate Through an Array with a For Loop
```js

```
## 26. 
```js

```
## 27. Constructing Strings with Variables
```js
var myStr = "My name is " + myName + " and I am well!";
```
## 28. Appending Variables to Strings
```js
var someAdjective = "boring";
var myStr = "Learning to code is ";
myStr += someAdjective;
```
## 29. Find the Length of a String
```js
lastNameLength = lastName.length;
```
## 30. Use Bracket Notation to Find the First Character in a String
```js
firstLetterOfLastName = lastName[0];
```
## 31. Understand String Immutability
String values are *immutable*, means that they cannot be altered once created.
```js
myStr = "Hello World";
```
## 32. Use Bracket Notation to Find the Nth Character in a String
```js
var thirdLetterOfLastName = lastName[2];
```
## 33. Use Bracket Notation to Find the Last Character in a String
Use  ```.length-1```
```js
var lastLetterOfLastName = lastName[lastName.length-1];
```
## 34. Use Bracket Notation to Find the Nth-to-Last Character in a String
```js
var secondToLastLetterOfLastName = lastName[lastName.length - 2];
```
## 35. Word Blanks
```js
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
  var result = "The " + myAdjective + " " + myNoun + " " + myVerb + " " + myAdverb + ".";
  return result;
}
wordBlanks("cat", "little", "hit", "slowly");
```
## 36. Store Multiple Values in one Variable using JavaScript Arrays
Array variables for storing several pieces of data in one place.
```js
var myArray = ["Alfi", 28];
```
## 37. Nest one Array within Another Array
```js
var myArray = [["Bulls", 23], ["White Sox", 45]];
```
## 39. Modify Array Data With Indexes
```js
myArray[0] = 45;
```
## 40. Access Multi-Dimensional Arrays With Indexes
```js
var myData = myArray[2][1];
```
## 41. Manipulate Arrays With push()
Adding an extra to the last array.
```js
myArray.push(["dog", 3]);
```
## 42. Manipulate Arrays With pop()
You can pop off the last array, and store it in a variable.
```js
var removedFromMyArray = myArray.pop();
```
## 43. Manipulate Arrays With shift()
removing the first in the array
```js
var removedFromMyArray = myArray.shift();
```
## 44. Manipulate Arrays With unshift()
Adding an extra to the first in the array.
```js
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

myArray.unshift(["Paul",35]);
```
## 45. Shopping List
```js
var myList = [["rice", 5] , ["bread", 6] , ["cake", 7], [ "quinoa", 9], ["potato", 20]];
```
## 46. Write Reusable JavaScript with Functions
```js
function reusableFunction() {
  console.log("Hi World");
}

reusableFunction();
```
## 47. Passing Values to Functions with Arguments
```js
function functionWithArgs (a , b) {
console.log(a + b);
}
functionWithArgs (1 , 2);
functionWithArgs (7 , 9);
```
## 48. Global Scope and Functions
Scope refers to the visibility of variables.
Variables which are defined **outside of a function block** have **Global scope**.
Variables which are used **without the ```var```** keyword are automatically created in the ```global``` scope. This can create unintended consequences elsewhere in your code or when running a function again. You should always declare your variables with ```var```.
```js
var myGlobal = 10;
function fun1() {
  oopsGlobal = 5;
}
```
## 49. Local Scope and Functions
```js
function myLocalScope() {
var myVar = 'use strict';
}
myLocalScope();
```
## 50. Global vs. Local Scope in Functions
```js
var outerWear = "T-Shirt";
function myOutfit() {
  var outerWear = "sweater";
  return outerWear;
}
myOutfit();
```
## 51. Return a Value from a Function with Return
Use a ```return``` statement to send a value back out of a function.
```js
function timesFive (num) {
  return num * 5;
}
timesFive(5);
timesFive(2);
timesFive(0);
```
## 52. Understanding Undefined Value returned from a Function
```js
function addFive() {
  sum = sum + 5;
}
```
## 53. Assignment with a Returned Value
```js
var processed = 0;
function processArg(num) {
  return (num + 3) / 5;
}
processed = processArg(7);
```
## 54. Stand in Line
 A **queue** is an abstract Data Structure where items are kept in order.
 New items can be added (```push```) at the back of the queue and old items are taken off (```shift```) from the front of the queue.

Add the number to the end of the array = ```push```
Remove the first element of the array = ```shift```
Then return the element that was removed = using ```return```.
```js
function nextInLine(arr, item) {
  arr.push(item);
  return  arr.shift();
}
```
## 55. Understanding Boolean Values
```js
function welcomeToBooleans() {
return true;
}
```
## 56. Use Conditional Logic with If Statements
```js
function trueOrFalse(wasThatTrue) {
    if (wasThatTrue) {
    return "Yes, that was true";
  }
  return "No, that was false";
}
trueOrFalse(true);
```
## 57. Comparison with the Equality Operator
```js
function testEqual(val) {
  if (val == 12) {
    return "Equal";
  }
  return "Not Equal";
}
testEqual(12);
```
## 58. Comparison with the Strict Equality Operator
However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a type conversion.

If the values being compared have different types, they are considered unequal, and the strict equality operator will return false.
```js
function testStrict(val) {
  if (val === 7) {
    return "Equal";
  }
  return "Not Equal";
}
testStrict(10);
```
## 59. Practice comparing different values
```js
function compareEquality(a, b) {
  if (a === b) {
    return "Equal";
  }
  return "Not Equal";
}
compareEquality(10, "10");
```
## 60. Comparison with the Inequality Operator
```js
function testNotEqual(val) {
  if (val != 99) {
    return "Not Equal";
  }
  return "Equal";
}
testNotEqual(10);
```
## 61. Comparison with the Strict Inequality Operator
```js
function testStrictNotEqual(val) {
  if (val !== 17) {
    return "Not Equal";
  }
  return "Equal";
}

testStrictNotEqual(10);
```
## 62. Comparison with the Greater Than Operator
```js
function testGreaterThan(val) {
  if (val > 100) {
    return "Over 100";
  }

  if (val > 10) {
    return "Over 10";
  }

  return "10 or Under";
}

testGreaterThan(10);
```
## 63. Comparison with the Greater Than Or Equal To Operator
```js
function testGreaterOrEqual(val) {
  if (val >= 20) {
    return "20 or Over";
  }

  if (val >= 10) {
    return "10 or Over";
  }

  return "Less than 10";
}


testGreaterOrEqual(10);
```
## 64. Comparison with the Less Than Operator
```js
function testLessThan(val) {
  if (val < 25) {
    return "Under 25";
  }

  if (val < 55) {
    return "Under 55";
  }

  return "55 or Over";
}

testLessThan(10);
```
## 65. Comparison with the Less Than Or Equal To Operator
```js
function testLessOrEqual(val) {
  if (val <= 12) {
    return "Smaller Than or Equal to 12";
  }

  if (val <=24) {
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}

testLessOrEqual(10);

```
## 66. Comparison with the Logical And Operator
```js
function testLogicalAnd(val) {

  if (val >= 25 && val <= 50) {
      return "Yes";
  }

  return "No";
}


testLogicalAnd(10);
```
## 67. Comparison with the Logical Or Operator
```js
function testLogicalOr(val) {


  if (val < 10 || val > 20 ) {

    return "Outside";
  }

  return "Inside";
}


testLogicalOr(15);
```
## 68. Introducing Else Statements

```js
function testElse(val) {
  var result = "";

  if (val > 5) {
    result = "Bigger than 5";
  }

  else {
    result = "5 or Smaller";
  }


  return result;
}


testElse(4);

```
## 69. Introducing Else If Statements
```js
function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }

  else if (val < 5) {
    return "Smaller than 5";
  }
  else {
      return "Between 5 and 10";
  }

}

testElseIf(7);

```
## 70. Logical Order in If Else Statements
```js
function orderMyLogic(val) {
  if (val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
}

orderMyLogic(7);
```
## 71. Chaining If Else Statements
```js
function testSize(num) {
  if(num < 5) {
    return "Tiny";
  } else if (num < 10) {
 return "Small";
  } else if (num < 15) {
return "Medium";
  } else if (num < 20) {
return "Large";
  } else if ( num >= 20 ) {
    return "Huge";
    } else {
    return "Change Me"; }

}

testSize(7);
```
## 72. Golf Code
```js
var names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];
function golfScore(par, strokes) {
  if (strokes == 1) {
return "Hole-in-one!";
  } else if (strokes <= par - 2) {
     return "Eagle" ;
  } else if (strokes == par - 1) {
     return "Birdie" ;
  } else if (strokes == par) {
     return "Par" ;
  } else if (strokes == par + 1) {
     return "Bogey" ;
  } else if (strokes == par + 2) {
     return "Double Bogey" ;
  } else if (strokes >= par + 3) {
     return "Go Home!" ;
  } else {
     return "Change Me";
  }
}

golfScore(5, 4);
```
