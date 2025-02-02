> begin [the debugging exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/debugging) and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD)  (wrong exercises, correct markdown styling)

[My FreeCodeCamp Portfolio](https://www.freecodecamp.org/fatmasumer)

### note for me: this framework is not correct. make yours.

## 1. Use the JavaScript Console to Check the Value of a Variable

```js
let a = 5;
let b = 1;
a++;
// Add your code below this line

console.log(a);
let sumAB = a + b;
console.log(sumAB);
```

## 2. Declare Variables
```js
var myName;
```

## 3.Storing Values with the Assignment Operator
```js
a = 7;
b = a;
a = b;
```

## 4. Initializing Variables with the Assignment Operator
```js
var a = 9;
```

## 5. Understanding Uninitialized Variables
```js
var a = 5;
var b = 10;
var c = "I am a";
```
## 6. Understanding Case Sensitivity in Variables
```js
// Declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Assignments
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```

## 7.Add Two Numbers (+)
```js
var sum = 10 + 0;
sum = 10 + 10;
```
## 8. Subtract One Number from Another
```js
var difference = 45 - 33;
```
## 9. Multiply Two Numbers
```js
var product = 8 * 10;
```
## 10. Divide One Number by Another (/)
```js
var quotient = 66 / 33;
```
## 11 .Increment a Number (i++)

```js
var myVar = 87;
myVar++;
```

## 12. Decrement a Number (i--)
```js
myVar--;
```


## 13. Create Decimal Numbers
```js
var myDecimal = 8.8;
```

## 14. Multiply Two Decimals
```js
var product = 2.0 * 2.5;
```

## 15. Divide One Decimal by Another
```js
var quotient = 4.4 / 2.0;
```
## 16. Finding a Remainder
```js
var remainder;
remainder = 11 % 3;
```
## 17. Compound Assignment With Augmented Addition (+=)
```js
a += 12;
b += 9;
c += 7;
```
## 18. Compound Assignment With Augmented Subtraction (-=)

```js
a -= 6;
b -= 15;
c -= 1;
```
## 19. Compound Assignment With Augmented Multiplication
```js
a *= 5;
b *= 3;
c *= 10;
```
## 20. Compound Assignment With Augmented Division
```js
a /= 12;
b /= 4;
c /= 11;
```

## 21. Declare String Variables
with  ``` " "  ```
```js
var myFirstName = "Alfi";
var myLastName = "Yusrina";
```

## 22. Escaping Literal Quotes in Strings
Using *backlash* ```\``` in the beginning and in the end of your quotes.
```js
var myStr = "I am a \"double quoted\" string inside \"double quotes\".";
```
## 23. Quoting Strings with Single Quotes
String values in JS may be written with single or double quotes.
```js
var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```

## 24. Escape Sequences in Strings
Reasons to use escaping characters:
- is to allow you to use characters you might not otherwise be able to type out, such as a backspace.
- is to allow you to represent multiple quotes in a string without JS misinterpreting what you mean.

```js
var myStr = 'FirstLine\n\t\\SecondLine\nThirdLine';
```

## 25. Concatenating Strings with Plus Operator
```js
var myStr = "This is the start. " +  "This is the end.";
```
## 26. Concatenating Strings with the Plus Equals Operator
```js
var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
```
