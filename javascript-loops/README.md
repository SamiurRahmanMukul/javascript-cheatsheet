# JavaScript Loops CheatSheet

## For Loop

```javascript
// Syntax: for (initialization; condition; update) { /* code to be executed */ }

// Example 1: Print numbers 1 to 5
for (let i = 1; i <= 5; i++) {
  console.log(i);
}

// Example 2: Sum of numbers 1 to 10
let sum = 0;
for (let i = 1; i <= 10; i++) {
  sum += i;
}
console.log("Sum:", sum);
```

## While Loop

```javascript
// Syntax: while (condition) { /* code to be executed */ }

// Example 3: Countdown from 5 to 1
let count = 5;
while (count > 0) {
  console.log(count);
  count--;
}

// Example 4: Calculate factorial of 5
let factorial = 1;
let num = 5;
while (num > 0) {
  factorial *= num;
  num--;
}
console.log("Factorial:", factorial);
```

## Do-While Loop

```javascript
// Syntax: do { /* code to be executed */ } while (condition);

// Example 5: Roll a dice until 6 is obtained
let diceResult;
do {
  diceResult = Math.ceil(Math.random() * 6);
  console.log("Dice:", diceResult);
} while (diceResult !== 6);

// For...In Loop (For Objects)
// Syntax: for (variable in object) { /* code to be executed */ }

// Example 6: Iterate over object properties
const person = { name: "John", age: 30, city: "New York" };
for (let key in person) {
  console.log(`${key}: ${person[key]}`);
}
```

## For...Of Loop (For Iterables)

```javascript
// Syntax: for (variable of iterable) { /* code to be executed */ }

// Example 7: Iterate over an array
const colors = ["red", "green", "blue"];
for (let color of colors) {
  console.log(color);
}

// Nested Loops
// Example 8: Multiplication Table (2x2 to 10x10)
for (let i = 2; i <= 10; i++) {
  console.log(`Multiples of ${i}:`);
  for (let j = 1; j <= 10; j++) {
    console.log(`${i} x ${j} = ${i * j}`);
  }
}
```

## Loop Control Statements

```javascript
/// break Statement
// Terminates the loop and transfers control to the statement following the loop
for (let i = 0; i < 5; i++) {
  if (i === 3) {
    break;
  }
  console.log(i);
}

/// continue Statement
// Skips the current iteration and continues to the next iteration
for (let i = 0; i < 5; i++) {
  if (i === 2) {
    continue;
  }
  console.log(i);
}
```
