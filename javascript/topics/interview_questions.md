# JavaScript Interview Questions

## Key Concepts
- JavaScript interviews test language fundamentals, DOM, async, ES6+, and problem-solving skills.

## Real-World Examples & Questions

### Example 1: Reverse a String
```javascript
function reverseString(str) {
  return str.split('').reverse().join('');
}
```

### Example 2: Debounce Function
```javascript
function debounce(fn, delay) {
  let timer;
  return function(...args) {
    clearTimeout(timer);
    timer = setTimeout(() => fn.apply(this, args), delay);
  };
}
```

### Example 3: Deep Clone an Object
```javascript
function deepClone(obj) {
  return JSON.parse(JSON.stringify(obj));
}
```

### Example 4: Real-time: How do you handle API errors in a React app?
A: Use try-catch in async functions, show user-friendly messages, and log errors for debugging.

### Example 5: Real-time: How do you optimize a large list rendering in the browser?
A: Use windowing/virtualization libraries (like react-window), lazy loading, and efficient DOM updates.

## Interview Q&A with Explanations

**Q1: What is closure in JavaScript?**
A: A closure is a function that retains access to its lexical scope even when executed outside that scope.

**Q2: Explain event delegation.**
A: Event delegation uses a single event listener on a parent element to handle events for multiple child elements, improving performance.

**Q3: What is the difference between `==` and `===`?**
A: `==` allows type coercion; `===` checks both value and type.

**Q4: Real-time: How do you prevent memory leaks in JavaScript apps?**
A: Remove event listeners, clear timers, and avoid global variables.

**Q5: Real-time: How do you handle asynchronous operations in loops?**
A: Use async/await with `for...of` or `Promise.all` for parallel execution.

## References
- [JavaScript Interview Questions - LeetCode](https://leetcode.com/problemset/all/?topicSlugs=javascript)
- [JavaScript.info: Interview](https://javascript.info/)
- [MDN: JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
