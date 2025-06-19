# jQuery Events

## Key Concepts
- jQuery simplifies event handling for clicks, hovers, form submissions, and more.
- Methods: `.on()`, `.click()`, `.hover()`, `.submit()`, `.keydown()`, `.off()`.

## Real-World Examples

### Example 1: Click Event
```javascript
$('#btn').click(function() {
  alert('Button clicked!');
});
```

### Example 2: Delegated Event Handling
```javascript
$('ul').on('click', 'li', function() {
  $(this).toggleClass('selected');
});
```

### Example 3: Form Submission
```javascript
$('form').submit(function(e) {
  e.preventDefault();
  alert('Form submitted!');
});
```

### Example 4: Hover Event
```javascript
$('.menu').hover(
  function() { $(this).addClass('hovered'); },
  function() { $(this).removeClass('hovered'); }
);
```

## Interview Questions & Answers

**Q1: How do you attach a click event to a button?**
A: Use `$('#btn').click(function(){ ... })` or `.on('click', ...)`.

**Q2: Real-time: How do you handle events for dynamically added elements?**
A: Use event delegation with `.on()` on a parent element.

**Q3: How do you prevent the default action of an event?**
A: Use `event.preventDefault()` in the handler.

## References
- [jQuery Events](https://api.jquery.com/category/events/)
- [jQuery Learning Center: Events](https://learn.jquery.com/events/)
