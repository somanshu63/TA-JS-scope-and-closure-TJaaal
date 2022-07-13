1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function(marks, total) {
    return (marks * 100) / total;
}
let percentage = (marks, total) => {
    return (marks * 100) / total;
}

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
function expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
function expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
  ```js
  it allows us to create anonymous function which does not have any name and can be executed much faster than function declaration
  let multiply = (numa, numb) => (numa * numb);
  ``` 

4. Why is a function call an expression in JavaScript?
  ```js
  because it executes the function with passed arguments and store it to any variable as a result.
  ```
5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // valid it will store the result of function add(2, 3).
five = add; // valid this will store the function reference
five = five(10, 11); // invalid as there is not function with five
five = function () {
  return 'Hello';
}; // valid function reference will be stored then we can execute it later
```

6. What is the difference between function definition and function call? Explain with an example.
```js
function add(a, b) {
  return a + b;
} // this is a function definition
this declares the function that what it has to do

add(1,4)//this is a function call
this executes(run) the function with the arguments passed to it 
```

7. What is the similarities between function definition and function call?
```js
both are codes that perform operations and return result
```

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // invalid
```

9. What is higher order function explain with an example.
```js
a function that accepts function as argument and returns a function
const randomNumbers = [4, 11, 42, 14, 39];
const filteredArray = randomNumbers.filter(n => {  
  return n > 5;
});
```

10. Explain what is callback function. Why you can pass a function inside a function?
```js
any function that is passed as an argument so that it can be executed in another function 
so that one can get the result from single function only
```