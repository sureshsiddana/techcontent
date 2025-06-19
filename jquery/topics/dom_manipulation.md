# jQuery DOM Manipulation

## Key Concepts
- jQuery makes it easy to get, set, and change DOM elements and their content.
- Methods: `.html()`, `.text()`, `.val()`, `.attr()`, `.append()`, `.prepend()`, `.remove()`, `.empty()`.

## Real-World Examples

### Example 1: Change HTML Content
```javascript
$('#info').html('<b>Updated!</b>');
```

### Example 2: Add Element to List
```javascript
$('ul').append('<li>New Item</li>');
```

### Example 3: Remove Element
```javascript
$('.ad-banner').remove();
```

### Example 4: Get and Set Attributes
```javascript
$('img').attr('alt', 'New description');
let src = $('img').attr('src');
```

## Interview Questions & Answers

**Q1: How do you change the text of an element?**
A: Use `.text('new text')`.

**Q2: Real-time: How do you add a new row to a table?**
A: Use `.append()` on the table body:
```javascript
$('table tbody').append('<tr><td>Data</td></tr>');
```

**Q3: How do you remove all child elements?**
A: Use `.empty()`.

## References
- [jQuery DOM Manipulation](https://api.jquery.com/category/manipulation/)
- [jQuery Learning Center: Manipulation](https://learn.jquery.com/using-jquery-core/manipulating-elements/)
