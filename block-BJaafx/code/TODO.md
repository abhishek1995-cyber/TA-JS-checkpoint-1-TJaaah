1. Using loops take 10 inputs from user and find the average of all the numbers.
 
function average(numbers) {
let total = 0
  for(i = 1; i <= numbers; i++) {
  let user = +prompt("inputs")
   total += user;
  } return total /numbers;
}
average(10)

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
Uncaught ReferenceError: println is not defined;

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum (max = 10) {
  let sum = 0
for (let i = 1; i <= max; i++) {
  if(i%2 == 0) {
    sum += i
  } 
} return sum;
}
```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum (max = 10) {
  let sum = 0
for (let i = 1; i <= max; i++) {
  if(i%2 != 0) {
    sum += i
  } 
} return sum;
}
```
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js
function getProductOfDigits(num) {
  let rem = 0;
 let product = 1;
  while(num > 0) {
   rem = num % 10;
   product *= rem;
   num = Math.floor(num / 10); 
  } return product
}
6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // 'Bigger than 5'
check(1); // 'Smaller than 5'
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // what will be the output
`you are arya`
getOutput('John'); // what will be the output
`you are john`
getOutput(); // what will be the output
`who are you
```
the reason here for the output is that every statement has seperate return so it return what condition is given

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 
You are arya
'Who are you'
getOutput('John'); // what will be the output
you are john
`who are you`
getOutput(); // what will be the output
`who are you`
```
the reason here for the output is that  every satetment has common return so after printing console.log it will also return the value provided.


9. Can a function have multiple return statement? Give one example if possible and explain the reason.

A function can have multiple return statements but only one of them will be executed because once a return statement is executed, the program control moves back to the caller function skipping the remaining statements of the current function.

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

for loop provides a concise way of writing the loop structure. Unlike a while loop, a for statement consumes the initialization, condition and increment/decrement in one line thereby providing a shorter, easy to debug structure of looping while A while loop is a control flow statement that allows code to be executed repeatedly based on a given Boolean condition. The while loop can be thought of as a repeating if statement.

example for loop
```js
int main()
{
  
    int i = 0;
  
    for (i = 5; i < 10; i++) {
        printf("GFG\n");
    }
  
    return 0;
}
```
example while loops
```js
nt main()
{
  
    int i = 5;
  
    while (i < 10) {
        printf("GFG\n");
        i++;
    }
  
    return 0;
}
````
