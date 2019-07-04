> start (and try to finish) the [object tasks](https://javascript.info/object) from javascript.info and paste each of your solutions into this file.    
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

### Create an empty object 'user'.
```js
var user = {}
```
### Add the property 'name' with the value 'John'.
```js
user.name = "John";
```

### Add the property surname with the value Smith.
```js
user.surname = "Smith";
```

### Change the value of the name to Pete.
user.name = "Pete"; 

### Remove the property name from the object.
```js
delete user.name; 
```

### Write the function isEmpty(obj) which returns true if the 
```js
function isEmpty(obj) {
  for (let key in obj) {
    return false;
  }
  return true;
}
```
### Constant objects?
Is it possible to change an object declared with const? What do you think?
```js
const user = {
  name: "John"
};

// does it work?
user.name = "Pete";
```
Yes, we can change it. 

### Sum object properties
Write the code to sum all salaries and store in the variable sum. Should be 390 in the example above. If salaries is empty, then the result must be 0.

```js
let salaries = {
  John: 100,
  Ann: 160,
  Pete: 130 }
  
  let sum = 0; 
  for (let key in salaries) {
  sum += salaries[key];
  }
  console.log(sum);
  
```
### Multiply numeric properties by 2
Create a function multiplyNumeric(obj) that multiplies all numeric properties of obj by 2. Please note that multiplyNumeric does not need to return anything. It should modify the object in-place.

```js
let menu = {
  width: 200,
  height: 300,
  title: "My menu"
};

function multiplyNumeric(obj) {
  for (let key in obj) {
    if (typeof obj[key] == 'number') {
      obj[key] *= 2;
    }
  }
}
multiplyNumeric(menu);

```
