# JavaScript Regular Expressions

## Key Concepts
- Regular expressions (regex) are patterns for matching character combinations in strings.
- Used for validation, searching, and replacing text.
- Syntax: `/pattern/flags`

## Real-World Examples

### Example 1: Testing a Pattern
```javascript
let re = /hello/i;
console.log(re.test('Hello world')); // true
```

### Example 2: Extracting Matches
```javascript
let str = 'abc123';
let result = str.match(/\d+/); // ['123']
```

### Example 3: Replacing Text
```javascript
let text = 'foo bar';
let newText = text.replace(/bar/, 'baz'); // 'foo baz'
```

## Interview Questions & Answers

**Q1: What is a regular expression?**
A: A sequence of characters that forms a search pattern, used for string matching and manipulation.

**Q2: Real-time: How do you validate an email address with regex?**
A: Use a pattern like `/^[\w.-]+@[\w.-]+\.\w+$/`.

**Q3: What does the `g` flag do?**
A: Global search; finds all matches, not just the first.

## References
- [MDN: RegExp](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)
- [JavaScript.info: RegExp](https://javascript.info/regexp-introduction)
