# JavaScript Object Methods CheatSheet

```javascript
const obj = { name: "John", age: 25, city: "New York" };
```

| Methods                | Code Example                                        | Result                                                      | Return Type     |
| ---------------------- | --------------------------------------------------- | ----------------------------------------------------------- | --------------- |
| Object.keys()          | Object.keys(obj)                                    | ["name", "age", "city"]                                     | array           |
| Object.values()        | Object.values(obj)                                  | ["John", 25, "New York"]                                    | array           |
| Object.entries()       | Object.entries(obj)                                 | [["name", "John"], ["age", 25], ["city", "New York"]]       | array of arrays |
| hasOwnProperty()       | obj.hasOwnProperty('age')                           | true                                                        | boolean         |
| propertyIsEnumerable() | obj.propertyIsEnumerable('city')                    | true                                                        | boolean         |
| Object.assign()        | Object.assign({}, obj, { gender: 'Male' })          | { name: 'John', age: 25, city: 'New York', gender: 'Male' } | object          |
| Object.freeze()        | Object.freeze(obj)                                  | (obj is now immutable)                                      | object          |
| Object.seal()          | Object.seal(obj)                                    | (obj is now sealed)                                         | object          |
| Object.keys()          | Object.keys(obj)                                    | ["name", "age", "city"]                                     | array           |
| Object.values()        | Object.values(obj)                                  | ["John", 25, "New York"]                                    | array           |
| Object.entries()       | Object.entries(obj)                                 | [["name", "John"], ["age", 25], ["city", "New York"]]       | array of arrays |
| Object.fromEntries()   | Object.fromEntries([['name', 'John'], ['age', 25]]) | { name: 'John', age: 25 }                                   | object          |
| delete                 | delete obj.age                                      | (removes 'age' property)                                    | boolean         |
| toString()             | obj.toString()                                      | "[object Object]"                                           | string          |
| hasOwnProperty()       | obj.hasOwnProperty('age')                           | true                                                        | boolean         |
| Object.keys()          | Object.keys(obj)                                    | ["name", "age", "city"]                                     | array           |
| Object.values()        | Object.values(obj)                                  | ["John", 25, "New York"]                                    | array           |
| Object.entries()       | Object.entries(obj)                                 | [["name", "John"], ["age", 25], ["city", "New York"]]       | array of arrays |
