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

A common task in JavaScript is to iterate through the contents of an array. One way to do that is with a for loop. 
First myArr and total are declared. Then the for loop starts. First i = 0, this is smaller than myArr.length (which is 5) so it will run the code inside the brackets: total += myArr[i] with i = 0, so: total += myArr[0] and myArr[0] = 2: total += 2. So now 2 is added to the total variable which is now 2 (0+2). Now i is incremented by 1 and becomes 1. Since this is smaller than myArr.length it will run the code between the brackets. Again it will add myArr[i], which is: myArr[1] which is: 3 to total variable. total is now 5 (2+3). These steps continue till myArr[4] has been added. Then i will become 5 and will no longer satisfy the condition (i < myArr.length).
```js
var myArr = [ 2, 3, 4, 5, 6];
var total = 0; 

for (var i = 0; i < myArr.length; i++) {
  total += myArr[i];
}
// Only change code below this line


```
## 26. Nesting For Loops
```js
function multiplyAll(arr) {
  var product = 1;
 
  for (var i = 0; i < arr.length; i++) {
    for (var j = 0; j < arr[i].length; j++ ){
      product *= arr[i][j];
    }
  }
  // Only change code above this line
  return product;
}

multiplyAll([[1,2],[3,4],[5,6,7]]);

```
## 27. Iterate with JavaScript Do...While Loops
do...while loop behaves just as you would expect with any other type of loops, but essentially, a **do...while loop** ensures that the code inside the loop will run at least once. 
```js
var myArray = [];
var i = 10;

do {
  myArray.push(i);
  i++;
} while (i < 5);


```
## 28. Profile Lookup
```js
function lookUpProfile(name, prop){
// Only change code below this line

for (var x = 0; x < contacts.length; x++){
    if (contacts[x].firstName === name) {
        if (contacts[x].hasOwnProperty(prop)) {
            return contacts[x][prop];
        } else {
            return "No such property";
        }
    }
}
return "No such contact";
}
```
## 29. Generate Random Fractions with JavaScript
```js
function randomFraction() {

 var result = 0;  // Math.random() can generate 0. We don't want to     return a 0,
  while (result === 0) {  // so keep generating random numbers until we get one     that isn't 0
    result = Math.random();
  }

  return result;  

  // Only change code above this line.
}
```
## 30. Generate Random Whole Numbers with JavaScript
```js

var randomNumberBetween0and19 = Math.floor(Math.random() * 20);

function randomWholeNum() {

  // Only change code below this line.

  return Math.floor(Math.random() * 10);
}

```
## 31. Generate Random Whole Numbers within a Range

```js


function randomRange(myMin, myMax) {

  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin; // Change this line

}
var myRandom = randomRange(5, 15);



```
## 32. Use the parseInt Function
The parseInt() function parses a string and returns an integer. 
```js
function convertToInteger(str) {
  return parseInt(str);
}

convertToInteger("56");

```
## 33.  Use the parseInt Function with a Radix
```js
function convertToInteger(str) {
  return parseInt(str, 2)
}

convertToInteger("10011");
```
## 34. Use the Conditional (Ternary) Operator
The conditional operator, also called the ternary operator, can be used as a one line if-else expression.
The syntax is: condition ? statement-if-true : statement-if-false;

```js
function checkEqual(a, b) {
  return a == b ? true : false;
}

checkEqual(1, 2);
```
## 35. Use Multiple Conditional (Ternary) Operators
```js
function checkSign(num) {
  return (num > 0) ? "positive" : (num < 0) ? "negative" : "zero" ;

}

checkSign(10);

```

