# JavaScript Array Methods CheatSheet

```javascript
const arr = [1, 2, 3, 4, 5];
const newArr = [6, 7, 8, 9, 10];
```

| Methods       | Code Example                           | Result                          | Return Type |
| ------------- | -------------------------------------- | ------------------------------- | ----------- |
| concat()      | arr.concat(newArr)                     | [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] | array       |
| join()        | arr.join('-')                          | "1-2-3-4-5"                     | string      |
| pop()         | arr.pop()                              | 5                               | number      |
| push()        | arr.push(6)                            | 6                               | number      |
| reverse()     | arr.reverse()                          | [5, 4, 3, 2, 1]                 | array       |
| shift()       | arr.shift()                            | 1                               | number      |
| unshift()     | arr.unshift(0)                         | 6                               | number      |
| slice()       | arr.slice(1, 4)                        | [2, 3, 4]                       | array       |
| splice()      | arr.splice(2, 1, 'a', 'b')             | [3]                             | array       |
| indexOf()     | arr.indexOf(3)                         | 2                               | number      |
| lastIndexOf() | arr.lastIndexOf(3)                     | 2                               | number      |
| includes()    | arr.includes(3)                        | true                            | boolean     |
| every()       | arr.every(num => num > 0)              | true                            | boolean     |
| some()        | arr.some(num => num < 0)               | false                           | boolean     |
| filter()      | arr.filter(num => num % 2 === 0)       | [2, 4]                          | array       |
| map()         | arr.map(num => num \* 2)               | [2, 4, 6, 8, 10]                | array       |
| forEach()     | arr.forEach(num => console.log(num))   | logs each element               | undefined   |
| reduce()      | arr.reduce((acc, num) => acc + num, 0) | 15                              | any         |
| find()        | arr.find(num => num > 2)               | 3                               | any         |
| findIndex()   | arr.findIndex(num => num > 2)          | 2                               | number      |
| fill()        | arr.fill(0, 2, 4)                      | [1, 2, 0, 0, 5]                 | array       |
| sort()        | arr.sort((a, b) => a - b)              | [1, 2, 3, 4, 5]                 | array       |
| isArray()     | Array.isArray(arr)                     | true                            | boolean     |
