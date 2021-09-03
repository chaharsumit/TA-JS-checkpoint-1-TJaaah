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
The difference between these functions is that in the first function we actually return a value i.e., the sum of two numbers but in the second we just log the value in the console but never return anything so the function returns undefined.


2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

first will have value of a + b the actual sum of two numbers.
second will have a value of undefined as the second function did not return anything.



3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

The output will be 36 as the fist two arguments will be assigned into the parameters a and b but the third one is just an extra agrument which is of no use and is ignored.



4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

Yes we can store the first sum function in a variable as it will become a function expression and we can use add() to perform the sum operation on two numbers.


5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

function sayHello(name){
	return `Hello ${name}`;
}
sayHello("Arya");



6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
//"Hello, John" will be the output as the value of userName in let message = `Hello, ` + userName is taken from our global variable userName and + opertaor concatenates the two values.



7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // "John"

showMessage(); // "Hello, John"

alert(userName); // "John"
```


8. What is a Anonymous Function give example of three functions.

An anonymous function is a function type that has no name for it. It is used in function expressions or in arrow functions.
For Example, let add = (a,b) => a + b; the right hand side is an anonymous function that performs operation but has got no name for it.
let add = function (a,b){ return a + b; } this is also an anonymous function which is a part of function expression.
let add = (a,b) { return a + b; } this is another example it don't have even the function keyword but is still a valid expression.



9. Can function declaration be a Anonymous Function? Explain

No function declaration can't be an anonymous function as they are separate entities or memory locations which need a name for us to refer to them thus they should always have a name and can't be anonymous on the other hand the function expressions are variables so they have their memory space name as the variable name to refer to them thus the function expression can store anonymous function without any issue but declaration give an unexpected token error.



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
