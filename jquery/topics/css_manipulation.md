# jQuery CSS Manipulation

## Key Concepts
- jQuery can get and set CSS properties and classes.
- Methods: `.css()`, `.addClass()`, `.removeClass()`, `.toggleClass()`, `.hasClass()`.

## Real-World Examples

### Example 1: Set CSS Property
```javascript
$('#box').css('background-color', 'yellow');
```

### Example 2: Add/Remove Class
```javascript
$('p').addClass('highlight');
$('p').removeClass('highlight');
```

### Example 3: Toggle Class
```javascript
$('.menu').click(function() {
  $(this).toggleClass('open');
});
```

### Example 4: Check for Class
```javascript
if ($('#box').hasClass('active')) {
  // do something
}
```

## Interview Questions & Answers

**Q1: How do you change the color of an element?**
A: Use `.css('color', 'red')`.

**Q2: Real-time: How do you toggle a class on click?**
A: Use `.toggleClass()` in a click handler.

**Q3: How do you check if an element has a class?**
A: Use `.hasClass('className')`.

## References
- [jQuery CSS](https://api.jquery.com/category/css/)
- [jQuery Learning Center: CSS](https://learn.jquery.com/using-jquery-core/css/)
