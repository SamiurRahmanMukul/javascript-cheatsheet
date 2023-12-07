# JavaScript Operators CheatSheet

## Arithmetic Operators

```javascript
let a = 5;
let b = 3;
```

| Operator | Example | Result | Description         |
| -------- | ------- | ------ | ------------------- |
| +        | a + b   | 8      | Addition            |
| -        | a - b   | 2      | Subtraction         |
| \*       | a \* b  | 15     | Multiplication      |
| /        | a / b   | 1.6667 | Division            |
| %        | a % b   | 2      | Modulus (remainder) |
| ++       | a++     | 6      | Increment           |
| --       | b--     | 2      | Decrement           |

## Assignment Operators

```javascript
let x = 10;
let y = 5;
```

| Operator | Example | Result | Description               |
| -------- | ------- | ------ | ------------------------- |
| =        | x = y   | 5      | Assignment                |
| +=       | x += y  | 15     | Addition assignment       |
| -=       | x -= y  | 5      | Subtraction assignment    |
| \*=      | x \*= y | 50     | Multiplication assignment |
| /=       | x /= y  | 2      | Division assignment       |
| %=       | x %= y  | 0      | Modulus assignment        |

## Comparison Operators

```javascript
let p = 10;
let q = "10";
```

| Operator | Example | Result | Description           |
| -------- | ------- | ------ | --------------------- |
| ==       | p == q  | true   | Equal                 |
| ===      | p === q | false  | Strict equal          |
| !=       | p != q  | false  | Not equal             |
| !==      | p !== q | true   | Strict not equal      |
| >        | p > q   | false  | Greater than          |
| <        | p < q   | false  | Less than             |
| >=       | p >= q  | true   | Greater than or equal |
| <=       | p <= q  | true   | Less than or equal    |

## Logical Operators

```javascript
let r = true;
let s = false;
```

| Operator | Example | Result | Description |
| -------- | ------- | ------ | ----------- |
| &&       | r && s  | false  | Logical AND |
| ∣∣       | r ∣∣ s  | true   | Logical OR  |
| !        | !r      | false  | Logical NOT |

## Conditional (Ternary) Operator

```javascript
let age = 20;
```

| Operator | Example                       | Result  | Description           |
| -------- | ----------------------------- | ------- | --------------------- |
| ? :      | age >= 18 ? "Adult" : "Minor" | "Adult" | Ternary (conditional) |

## Bitwise Operators

```javascript
let t = 5; // 101 in binary
let u = 3; // 011 in binary
```

| Operator | Example | Result | Description |
| -------- | ------- | ------ | ----------- |
| &        | t & u   | 1      | Bitwise AND |
| \|       | t \| u  | 7      | Bitwise OR  |
| ^        | t ^ u   | 6      | Bitwise XOR |
| ~        | ~t      | -6     | Bitwise NOT |
| <<       | t << 1  | 10     | Left shift  |
| >>       | t >> 1  | 2      | Right shift |
