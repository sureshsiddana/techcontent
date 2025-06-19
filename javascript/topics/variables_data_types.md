# JavaScript Variables & Data Types

## Key Concepts
- Variables store data values. Declared with `var`, `let`, or `const`.
- Data types: string, number, boolean, null, undefined, object, symbol, bigint.
- `let` and `const` (ES6+) have block scope; `var` has function scope.

## Real-World Examples

### Example 1: Declaring Variables
```javascript
let name = 'Alice';
const PI = 3.14159;
var age = 30;
```

### Example 2: Data Types
```javascript
let str = 'Hello'; // string
let num = 42;      // number
let isActive = true; // boolean
let obj = { key: 'value' }; // object
let arr = [1, 2, 3]; // array (object)
let n = null; // null
let u; // undefined
```

### Example 3: Type Checking
```javascript
console.log(typeof str); // 'string'
console.log(typeof arr); // 'object'
```

## Interview Questions & Answers

**Q1: What is the difference between `let`, `const`, and `var`?**
A: `let` and `const` are block-scoped (ES6+), `var` is function-scoped. `const` cannot be reassigned.

**Q2: Real-time: How do you check if a variable is undefined?**
A: Use `typeof` or strict equality:
```javascript
if (typeof x === 'undefined') { /* ... */ }
```

**Q3: What is the difference between `null` and `undefined`?**
A: `null` is an assigned value meaning "no value"; `undefined` means a variable has been declared but not assigned.

## References
- [MDN: var, let, const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)
- [JavaScript.info: Variables](https://javascript.info/variables)
