# JavaScript Number Methods CheatSheet

```javascript
const num = 123.456;
```

| Methods         | Code Example          | Result                         | Return Type |
| --------------- | --------------------- | ------------------------------ | ----------- |
| toExponential() | num.toExponential(2)  | "1.23e+2"                      | string      |
| toFixed()       | num.toFixed(2)        | "123.46"                       | string      |
| toPrecision()   | num.toPrecision(5)    | "123.46"                       | string      |
| toString()      | num.toString()        | "123.456"                      | string      |
| parseInt()      | parseInt("123.456")   | 123                            | number      |
| parseFloat()    | parseFloat("123.456") | 123.456                        | number      |
| isNaN()         | isNaN("hello")        | true                           | boolean     |
| isFinite()      | isFinite(10 / 0)      | false                          | boolean     |
| Math.round()    | Math.round(123.456)   | 123                            | number      |
| Math.ceil()     | Math.ceil(123.456)    | 124                            | number      |
| Math.floor()    | Math.floor(123.456)   | 123                            | number      |
| Math.abs()      | Math.abs(-123.456)    | 123.456                        | number      |
| Math.sqrt()     | Math.sqrt(144)        | 12                             | number      |
| Math.pow()      | Math.pow(2, 3)        | 8                              | number      |
| Math.min()      | Math.min(1, 2, 3)     | 1                              | number      |
| Math.max()      | Math.max(1, 2, 3)     | 3                              | number      |
| Math.random()   | Math.random()         | (random value between 0 and 1) | number      |
