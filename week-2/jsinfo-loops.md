> start (and try to finish) the [loop tasks](https://javascript.info/while-for) from javascript.info and paste each of your solutions into this file.  
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

### Last loop value
```js
let i = 3;

while (i) {
  alert( i-- );
}
```
What is the last value alerted by this code? Why?

It is 1. According to explanations while (i) is a shorter way to write while (i != 0). Here, the condition i !=0 means when i is not equal to zero. So, until i is zero these statements in the while block would be executed repeatedly. 

### Which values does the while loop show?

```js
let i = 0;
while (++i < 5) alert( i ); //The prefix form ++i:

let i = 0;
while (i++ < 5) alert( i ); //The postfix form i++
```
For every loop iteration, write down which value it outputs and then compare it with the solution. Both loops alert the same values, or not?

In the prefix form, the alert value is 1, then 2, 3, 4 respectively. In the postfix form, it again starts with 1 but ends with 5.   

### Which values get shown by the "for" loop?
```js
for (let i = 0; i < 5; ++i) alert( i );  //The prefix form

for (let i = 0; i < 5; i++) alert( i ); //The postfix form
```
In both loops, values start with 0 and end with 4. There’s no difference between i++ and ++i in for loops. 

### Output even numbers in the loop.
Use the for loop to output even numbers from 2 to 10.
```js
for (let i = 2; i <=10; i++) { 
    if (i % 2 == 0) continue; 
    console.log(i); }
```
### Replace "for" with "while"
Rewrite the code changing the for loop to while without altering its behavior (the output should stay same).
```js
for (let i = 0; i < 3; i++) {
  alert( `number ${i}!` );
}
```
```
let i = 0; 
undefined
do {alert( `number ${i}!`);  
    i++; }  
while (i < 3 ); 

```
OR
```
let i = 0;
while (i < 3) {
  alert( `number ${i}!` );
  i++;
}
```
### Repeat until the input is correct.
Write a loop which prompts for a number greater than 100. If the visitor enters another number – ask them to input again.The loop must ask for a number until either the visitor enters a number greater than 100 or cancels the input/enters an empty line. Here we can assume that the visitor only inputs numbers. There’s no need to implement a special handling for a non-numeric input in this task.

```js
let num;

do {
  num = prompt("Enter a number greater than 100?", 0);
} while (num <= 100 && num);

```
### Output prime numbers.

```js
let n = 10;

nextPrime:
for (let i = 2; i <= n; i++) { // for each i...

  for (let j = 2; j < i; j++) { // look for a divisor..
    if (i % j == 0) continue nextPrime; // not a prime, go next i
  }

  alert( i ); // a prime
}
```
