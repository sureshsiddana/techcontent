# jQuery Basics

## Key Concepts
- jQuery is a fast, small, and feature-rich JavaScript library.
- Simplifies HTML document traversal, event handling, and animation.
- Uses the `$` function to select and manipulate elements.

## Real-World Examples

### Example 1: Document Ready
```javascript
$(document).ready(function() {
  console.log('DOM is ready!');
});
```

### Example 2: Hide an Element
```javascript
$('#myDiv').hide();
```

### Example 3: Change Text
```javascript
$('#greet').text('Hello, jQuery!');
```

## Interview Questions & Answers

**Q1: What is jQuery and why is it used?**
A: jQuery is a JavaScript library that simplifies DOM manipulation, event handling, and AJAX.

**Q2: Real-time: How do you ensure code runs after the DOM is loaded?**
A: Use `$(document).ready()` or the shorthand `$(function(){ ... })`.

**Q3: How do you select an element by ID?**
A: Use `$('#elementId')`.

## References
- [jQuery Basics](https://learn.jquery.com/using-jquery-core/)
- [jQuery API](https://api.jquery.com/)
