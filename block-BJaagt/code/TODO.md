Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the scope and we can't access the variable defined inside a scope with let or const from outside.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the condition and we can't access the variable defined inside a condition with let or const from outside.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // "Arya"
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the condition and we can access the variable defined inside a condition with var from outside.

The above code will give the output `Arya`.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is variable named `username` in the global scope. also there is a variable inside the condition and we can access the variable defined inside a condition with var from outside so this will clash.

The above code will throw an error `SyntaxError: Identifier 'username' has already been declared`.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // `John`
```
In above code we are looking for the variable named `username`. There is a variable named `username` in the global scope. also there is a variable inside the condition and we can't access the variable defined inside a condition with let or const from outside so it will take the global variable show the output `John`.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // `John`
```
In above code we are looking for the variable named `username`. There is a variable named `username` in the global scope. also there is a variable inside the function sayHello and we can't access the variable defined inside a function from outside so it will take the global variable and show the output `John`.


8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 'First'
                           // 1 'First'
                           // 2 'First'
                           // 3 'First'
                           // 4 'First'
                           // 5 'First'
                           // 6 'First'
                           // 7 'First'
                           // 8 'First'
                           // 9 'First'
}
console.log(i, 'Second'); // 10 'Second'
```
in this the loop will run first and will give the output written above after completion of iteration it will make the value of i to 10 and as it was declared by var we can recieve on the outside also so the last console will recieve the value of 10 and show the output wriiten on second

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 'First'
                           // 1 'First'
                           // 2 'First'
                           // 3 'First'
                           // 4 'First'
                           // 5 'First'
                           // 6 'First'
                           // 7 'First'
                           // 8 'First'
                           // 9 'First'
}
console.log(i, 'Second'); //  ReferenceError: i is not defined
```
this is because we declared i with let due to which we cannot access it outside so it is showing error for the outside console
