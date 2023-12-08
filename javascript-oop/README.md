# JavaScript OOP (Object-Oriented Programming) CheatSheet

## Object Creation

```javascript
// Constructor Function
function Person(name, age) {
  this.name = name;
  this.age = age;
}

// Object Instance
const john = new Person("John", 30);
```

## Prototypes

```javascript
// Adding a method to the prototype of the constructor function
Person.prototype.greet = function () {
  return `Hello, my name is ${this.name} and I am ${this.age} years old.`;
};

console.log(person1.greet()); // Output: "Hello, my name is Alice and I am 30 years old."
console.log(person2.greet()); // Output: "Hello, my name is Bob and I am 25 years old."
```

## ES6 Class

```javascript
class Animal {
  constructor(name, sound) {
    this.name = name;
    this.sound = sound;
  }

  makeSound() {
    console.log(this.sound);
  }
}

// Class Instance
const cat = new Animal("Cat", "Meow");
```

## Inheritance

```javascript
// Prototypal Inheritance
function Employee(name, position) {
  this.name = name;
  this.position = position;
}

Employee.prototype.sayHello = function () {
  console.log(`Hello, I'm ${this.name}, a ${this.position}.`);
};

const manager = new Employee("Alice", "Manager");

// ES6 Class Inheritance
class Programmer extends Employee {
  constructor(name, position, language) {
    super(name, position);
    this.language = language;
  }

  code() {
    console.log(`Coding in ${this.language}`);
  }
}

const developer = new Programmer("Bob", "Developer", "JavaScript");
```

## Encapsulation

```javascript
// Using Closure
function Counter() {
  let count = 0;

  return {
    increment: function () {
      count++;
    },
    getCount: function () {
      return count;
    },
  };
}

const counter = Counter();
counter.increment();
console.log(counter.getCount()); // Output: 1

// Private Class Fields (ES6)
class BankAccount {
  #balance = 1000;

  getBalance() {
    return this.#balance;
  }

  deposit(amount) {
    this.#balance += amount;
  }

  withdraw(amount) {
    if (amount <= this.#balance) {
      this.#balance -= amount;
    } else {
      console.log("Insufficient funds");
    }
  }
}

const account = new BankAccount();
account.deposit(500);
account.withdraw(200);
console.log(account.getBalance()); // Output: 1300
```

## Polymorphism

```javascript
// Method Overriding
class Shape {
  area() {
    console.log("Area calculation not implemented.");
  }
}

class Circle extends Shape {
  constructor(radius) {
    super();
    this.radius = radius;
  }

  area() {
    console.log(`Area of Circle: ${Math.PI * this.radius ** 2}`);
  }
}

class Square extends Shape {
  constructor(side) {
    super();
    this.side = side;
  }

  area() {
    console.log(`Area of Square: ${this.side ** 2}`);
  }
}

const circle = new Circle(5);
const square = new Square(4);

circle.area(); // Output: Area of Circle: 78.53981633974483
square.area(); // Output: Area of Square: 16
```

<p align="start">
  This cheat sheet covers key Object-Oriented Programming concepts in JavaScript, including object creation, prototypes, inheritance, encapsulation, and polymorphism. Feel free to use it as a quick reference guide!
</p>
