# JavaScript Debugging & Best Practices

## Key Concepts
- Debugging uses browser DevTools, breakpoints, and console methods.
- Best practices: use `let`/`const`, avoid global variables, write modular code, handle errors, and comment wisely.

## Real-World Examples

### Example 1: Using console.log
```javascript
console.log('Debug info:', variable);
```

### Example 2: Setting Breakpoints
- Open browser DevTools (F12), go to Sources, click line number to set a breakpoint.

### Example 3: Linting with ESLint
- Use ESLint to catch errors and enforce code style.

## Interview Questions & Answers

**Q1: How do you debug JavaScript in the browser?**
A: Use DevTools (Console, Sources, Network), set breakpoints, inspect variables, and step through code.

**Q2: Real-time: How do you prevent common bugs in JavaScript?**
A: Use strict mode, linting tools, write tests, and follow best practices.

**Q3: What is the benefit of using `const` over `var`?**
A: `const` prevents reassignment and accidental bugs; `var` is function-scoped and can lead to hoisting issues.

## References
- [MDN: Debugging](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Debugging)
- [JavaScript.info: Debugging](https://javascript.info/debugging-chrome)
