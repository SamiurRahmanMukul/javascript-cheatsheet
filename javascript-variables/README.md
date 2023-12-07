# JavaScript Variables CheatSheet

## Declaration and Initialization

```javascript
let firstName = "John"; // Declaring and initializing a string variable
let age = 25; // Declaring and initializing a number variable
let isStudent = true; // Declaring and initializing a boolean variable
let grades = [90, 85, 92]; // Declaring and initializing an array variable

// Declaring and initializing an object variable
let person = {
  name: "Alice",
  age: 30,
};
```

## Variable Naming Rules

```javascript
let camelCaseVariable; // Camel case is commonly used (e.g., camelCase)
let snake_case_variable; // Snake case is an alternative (e.g., snake_case)
const PI = 3.14; // Constants are usually written in uppercase
```

## Scope

```javascript
function exampleFunction() {
  let localVar = "I am a local variable"; // Local variable within the function
  console.log(localVar);
}

exampleFunction(); // Output: "I am a local variable"
console.log(localVar); // Error: localVar is not defined outside the function
```

## Hoisting

```javascript
console.log(hoistedVar); // Output: undefined
var hoistedVar = "I am hoisted"; // Variable declaration is hoisted to the top
```

## Let, Const, and Var

```javascript
let user = "Alice"; // Block-scoped variable
const PI_VALUE = 3.14; // Constant variable
var globalVar = "I am global"; // Function-scoped variable (avoid using)
```

## Template Literals

```javascript
let message = `Hello, ${firstName}! You are ${age} years old.`;
console.log(message); // Output: "Hello, John! You are 25 years old."
```

## Dynamic Typing

```javascript
let dynamicVariable = "I am a string";
dynamicVariable = 42; // Can change type dynamically
console.log(dynamicVariable); // Output: 42
```

## Null and Undefined

```javascript
let nullVariable = null; // Represents intentional absence of any object value
let undefinedVariable; // Variable has been declared but not defined
console.log(nullVariable); // Output: null
console.log(undefinedVariable); // Output: undefined
```

## typeof Operator

```javascript
console.log(typeof age); // Output: "number"
console.log(typeof isStudent); // Output: "boolean"

// Examples
let x = 5;
let y = 10;
let sum = x + y; // Sum is 15
console.log(sum); // Output: 15
```

## Concatenating Strings

```javascript
let greeting = "Hello";
let name = "World";
let welcomeMessage = greeting + ", " + name + "!";
console.log(welcomeMessage); // Output: "Hello, World!"

// Array Operations
grades.push(88); // Adds 88 to the end of the grades array
console.log(grades); // Output: [90, 85, 92, 88]

// Object Properties
console.log(person.name); // Output: "Alice"
person.location = "City A"; // Adding a new property to the person object
console.log(person); // Output: { name: 'Alice', age: 30, location: 'City A' }
```
