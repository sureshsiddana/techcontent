# jQuery Effects & Animations

## Key Concepts
- jQuery provides simple methods for creating effects and animations.
- Common methods: `.hide()`, `.show()`, `.fadeIn()`, `.fadeOut()`, `.slideUp()`, `.slideDown()`, `.animate()`.

## Real-World Examples

### Example 1: Fade In/Out
```javascript
$('#box').fadeIn(500);
$('#box').fadeOut(500);
```

### Example 2: Slide Up/Down
```javascript
$('.panel').slideDown();
$('.panel').slideUp();
```

### Example 3: Custom Animation
```javascript
$('#move').animate({ left: '250px' }, 1000);
```

## Interview Questions & Answers

**Q1: How do you hide an element with animation?**
A: Use `.fadeOut()` or `.slideUp()`.

**Q2: Real-time: How do you chain multiple effects?**
A: Call methods in sequence:
```javascript
$('#box').fadeOut().fadeIn();
```

**Q3: How do you stop an animation before it completes?**
A: Use `.stop()`.

## References
- [jQuery Effects](https://api.jquery.com/category/effects/)
- [jQuery Learning Center: Effects](https://learn.jquery.com/effects/)
