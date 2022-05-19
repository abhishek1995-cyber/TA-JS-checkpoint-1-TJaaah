1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
if we call the first sum wel will get get sum of a and b as well as if we call second sum we get undefined as well as sum of a and b. but it both case we get undefined value as we in question function isnt called anywhere. 

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

  -  value of `first` we get undefined whereas for second we get sum of a and b as well as undefined

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

 - we will get the sum of a and b as we defined only two parameter above in the function so the third parameter while calling willbe ignored.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
 
 - yes we can store in a variable named add because function is a expression and we can store any expression in variables.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
 ```js
 function sayHello(name) {
   return `Hello Arya`;
 }
6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
-output will be `Hello, John` as function return variables from ourside also.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1  

showMessage(); // Output 2

alert(userName); // Output 3
``` 
- output 1 will alert john while it is undefined.
-output 2 will be `Hello, John`.
- output 1 will alert john while it is undefined.

8. What is a Anonymous Function give example of three functions.

-Anonymous Function is a function that does not have any name associated with it. Normally we use the function keyword before the function name to define a function in JavaScript, however, in anonymous functions in JavaScript, we use only the function keyword without the function name.
example - 1
```js
var anon = function() {
  alert('I am anonymous');
}
anon();
```
example-2 arrow function 
```js
var anon = x => x + 1
```
example-3 arrow with brackets
```js
var anon = x => {return x + 1}

9. Can function declaration be a Anonymous Function? Explain.

 - yes function declaration be a anonymous function by arrow operator as well as i had given example above.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
```js
function get() {
  return `return a value`
}
function calc() {
  return `calculate something`;
}
function create() {
  return `create something`
}
function check() {
  return `check something and return a boolean, etc`
}
function show() {
  return `show something`
}
