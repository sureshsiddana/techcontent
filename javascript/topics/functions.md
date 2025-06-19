# JavaScript Functions

## Key Concepts
- Functions are reusable blocks of code that perform a specific task.
- Declared with `function` keyword, arrow functions (ES6+), or as function expressions.
- Functions can return values and accept parameters.

## Real-World Examples

### Example 1: Function Declaration
```javascript
function greet(name) {
  return 'Hello, ' + name + '!';
}
console.log(greet('Alice'));
```

### Example 2: Arrow Function
```javascript
const add = (a, b) => a + b;
console.log(add(2, 3)); // 5
```

### Example 3: Function Expression
```javascript
const square = function(x) {
  return x * x;
};
console.log(square(4)); // 16
```

## Interview Questions & Answers

**Q1: What is the difference between a function declaration and a function expression?**
A: Declarations are hoisted; expressions are not. Declarations use `function name() {}`; expressions assign a function to a variable.

**Q2: Real-time: How do you pass a function as an argument?**
A: Functions are first-class citizens. Example:
```javascript
function process(fn) { fn(); }
process(() => console.log('Run!'));
```

**Q3: What is an arrow function?**
A: A concise syntax for writing functions, introduced in ES6. Does not have its own `this`.

## References
- [MDN: Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
- [JavaScript.info: Functions](https://javascript.info/function-basics)
