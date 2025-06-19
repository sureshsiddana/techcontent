# JavaScript Control Flow (if, switch, loops)

## Key Concepts
- Control flow structures determine the order in which code executes.
- Includes `if`, `else`, `switch`, `for`, `while`, and `do...while` loops.

## Real-World Examples

### Example 1: if-else Statement
```javascript
let age = 18;
if (age >= 18) {
  console.log('Adult');
} else {
  console.log('Minor');
}
```

### Example 2: switch Statement
```javascript
let day = 3;
switch(day) {
  case 1: console.log('Monday'); break;
  case 2: console.log('Tuesday'); break;
  case 3: console.log('Wednesday'); break;
  default: console.log('Other day');
}
```

### Example 3: for Loop
```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

### Example 4: while Loop
```javascript
let n = 3;
while (n > 0) {
  console.log(n);
  n--;
}
```

## Interview Questions & Answers

**Q1: What is the difference between `for` and `while` loops?**
A: `for` is used when the number of iterations is known; `while` is used when the condition is checked before each iteration and the number of iterations may not be known.

**Q2: Real-time: How do you break out of a loop early?**
A: Use the `break` statement.

**Q3: What is the purpose of the `continue` statement?**
A: Skips the current iteration and continues with the next one.

## References
- [MDN: Control Flow](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)
- [JavaScript.info: Loops](https://javascript.info/while-for)
