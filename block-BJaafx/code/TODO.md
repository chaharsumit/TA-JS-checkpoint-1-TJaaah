1. Using loops take 10 inputs from user and find the average of all the numbers.

let i = 10;
let sum = 0;
while(i){
	sum += +prompt(`enter a number`);
	i--;
}
let result = sum / 10;
console.log(result);


2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
// An error will be thrown as println method is not defined is javaScript it's a method in java.



3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

function getEvenSum(max = 10){
	let result = 0;
	for(let i = 1 ; i <= max; i++){
		if(i % 2 == 0){
			result += i;
		}
	}
	return result;
}

getEvenSum(20);

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
function getOddSum(max = 10){
	let result = 0;
	for(let i = 1 ; i <= max; i++){
		if(i % 2 != 0){
			result += i;
		}
	}
	return result;
}

getOddSum(20);



5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

function getProductOfDigits(num){
  i = 0;
  let result = 0;
  if(num > 0){
    while(i != num.length){
      result += +num[i];
      i++;
    }
    return result;
  }
  return `not a valid input`;
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

check(10); // "Bigger than 5"
check(1); // "Smaller than 5"
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'
getOutput('John'); // 'You are john'
getOutput(); // 'who are you'
```
The comparison happens in if condition and in the first two test cases it comes out to be true thus the expected outputs gets displayed but in the third test case the both if statements get false in return form its comparison operator so the third or default return is triggered.



8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'
getOutput('John'); // 'You are john'
getOutput(); // 'who are you'
```
The comparison happens in if condition and in the first two test cases it comes out to be true thus the expected outputs gets displayed but in the third test case the both if statements get false in return form its comparison operator so the third or default return is triggered.


9. Can a function have multiple return statement? Give one example if possible and explain the reason.
Yes a function can have multiple return statements as many as possible but there will always be only one return statement trigerred per function as whenever we parse a return statement the function's execution ends and a value is returned by the function.
for example;
	function isTrue(num){
		if(num == 0){
			return true;
		}
		return false;
	}

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
For and while both do the same work but are having their own use cases as we use for in case know the exact amount of iterations say we have to iterate over a small array with a given length whereas while loop is used in case we have large amount to data to iterate upon and we don't know when our conditional statement will become false to finally stop the loop.
The while loop has only one parameter in its parenthesis whereas in for you can have multiple expressions as parameters as for loop clearly specifies all the required information about the iteration before we start it.
For example, we have an array  arr = [1,2,3];
Now, we can iterate over it and say add its elements by both for and while as
	for(let i = 0 ; i < arr.length; i++){
		--------
	}
	while(i < arr.length){
		--------
		i++;
	}
	
	In both of these we can perform any operation over out array's length but the for loop makes more sense as in the body of our loop we only have the exact operation which we are going to do but in the while loop we could end up having additional statements in the loop body. Thus for a small task like above we should use for loop for better readability.


