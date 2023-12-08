# JavaScript Functions CheatSheet

## Declaration

```javascript
function functionName(parameters) {
  // Code to be executed when the function is called
  return result; // Optional: return a value
}
```

## Anonymous Function

```javascript
let anonymousFunction = function (parameters) {
  // Code to be executed
  return result;
};
```

## Arrow Function (ES6+)

```javascript
let arrowFunction = (parameters) => {
  // Code to be executed
  return result;
};
```

## Default Parameters

```javascript
function greet(name = "Guest") {
  return `Hello, ${name}!`;
}
console.log(greet()); // Output: "Hello, Guest!"
console.log(greet("John")); // Output: "Hello, John!"
```

## Rest Parameter

```javascript
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}
console.log(sum(1, 2, 3, 4, 5)); // Output: 15
```

## Spread Operator

```javascript
let array1 = [1, 2, 3];
let array2 = [4, 5, 6];
let mergedArray = [...array1, ...array2];
console.log(mergedArray); // Output: [1, 2, 3, 4, 5, 6]
```

## Closure

```javascript
function outerFunction() {
  let outerVariable = "I am outer";

  function innerFunction() {
    console.log(outerVariable); // Accessing outer variable
  }

  return innerFunction;
}

let closureFunction = outerFunction();
closureFunction(); // Output: "I am outer"
```

## Higher-Order Function

```javascript
function multiplyBy(factor) {
  return function (number) {
    return number * factor;
  };
}

let double = multiplyBy(2);
console.log(double(5)); // Output: 10
```

## Callback Function

```javascript
function fetchData(callback) {
  // Async operation, e.g., fetching data from an API
  let data = { name: "John", age: 30 };
  callback(data);
}

function handleData(data) {
  console.log(`Received data: ${JSON.stringify(data)}`);
}

fetchData(handleData);
```

## Immediately Invoked Function Expression (IIFE)

```javascript
(function () {
  // Code to be executed immediately
})();
```

## Function Expression vs Function Declaration

```javascript
declarationFunction(); // Hoisted, can be called before declaration
function declarationFunction() {
  console.log("I am a function declaration");
}

// expressionFunction(); // Error: expressionFunction is not defined before it's called
let expressionFunction = function () {
  console.log("I am a function expression");
};
```

## Arrow Function Shorthand

```javascript
let square = (x) => x * x;
console.log(square(4)); // Output: 16

// Note: Replace "functionName", "parameters", "result", etc., with actual values in your code.
```

## Parameters and Arguments

```javascript
/// Parameters: Variables declared in the function's definition

// Single Parameter
function greet(name) {
  console.log(`Hello, ${name}!`);
}

// Multiple Parameters
function addNumbers(a, b) {
  console.log(a + b);
}

// Default Parameters
function multiply(a, b = 2) {
  console.log(a * b);
}

// Rest Parameter
function sum(...numbers) {
  console.log(numbers.reduce((acc, num) => acc + num, 0));
}

/// Arguments: Actual values passed to a function when it is called

// Single Argument
greet("John");

// Multiple Arguments
addNumbers(3, 5);

// Default Parameter Usage
multiply(4); // Uses default value of b (2)

// Rest Parameter Usage
sum(1, 2, 3, 4, 5); // Outputs: 15

// Note: The number and order of arguments must match the number and order of parameters.

// Practical Examples

// Example 1: Function with parameters and arguments
function fullName(firstName, lastName) {
  console.log(`${firstName} ${lastName}`);
}

fullName("John", "Doe"); // Outputs: "John Doe"

// Example 2: Function with default parameter
function greetUser(userName = "Guest") {
  console.log(`Hello, ${userName}!`);
}

greetUser(); // Outputs: "Hello, Guest"
greetUser("Alice"); // Outputs: "Hello, Alice"

// Example 3: Function with rest parameter
function displayItems(category, ...items) {
  console.log(`Category: ${category}`);
  console.log("Items:", items);
}

displayItems("Electronics", "Laptop", "Phone", "Camera");
// Outputs:
// Category: Electronics
// Items: [ 'Laptop', 'Phone', 'Camera' ]
```
