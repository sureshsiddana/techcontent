# Asynchronous JavaScript (Callbacks, Promises, Async/Await)

## Key Concepts
- JavaScript is single-threaded but supports asynchronous operations (timers, AJAX, file I/O).
- Callbacks, Promises, and async/await are used for async code.

## Real-World Examples

### Example 1: Callback
```javascript
setTimeout(function() {
  console.log('Executed after 1 second');
}, 1000);
```

### Example 2: Promise
```javascript
let promise = new Promise((resolve, reject) => {
  setTimeout(() => resolve('Done!'), 1000);
});
promise.then(result => console.log(result));
```

### Example 3: Async/Await
```javascript
async function fetchData() {
  let response = await fetch('https://api.example.com/data');
  let data = await response.json();
  console.log(data);
}
fetchData();
```

## Interview Questions & Answers

**Q1: What is a callback?**
A: A function passed as an argument to another function, executed after an operation completes.

**Q2: Real-time: How do you handle errors in Promises?**
A: Use `.catch()` method:
```javascript
promise.catch(error => console.error(error));
```

**Q3: What is the advantage of async/await over Promises?**
A: async/await makes asynchronous code look synchronous and is easier to read and maintain.

## References
- [MDN: Asynchronous Programming](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous)
- [JavaScript.info: Async](https://javascript.info/async)
