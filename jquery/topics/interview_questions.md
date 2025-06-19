# jQuery Interview Questions (100+ Real-Time Scenarios)

## Key Concepts
- jQuery interviews test DOM manipulation, selectors, events, AJAX, plugins, and best practices.
- Real-world scenarios focus on debugging, optimization, and integration with modern JavaScript.

---

### 1. What is jQuery and why is it used?
**A:** jQuery is a JavaScript library that simplifies HTML DOM manipulation, event handling, and AJAX. It is used for concise, cross-browser code.

### 2. How do you select all elements with a specific class?
**A:** Use `$('.className')`.

### 3. How do you hide and show an element?
**A:** Use `.hide()` and `.show()` methods.

### 4. Real-time: How do you add a click event to dynamically created elements?
**A:** Use event delegation:
```javascript
$('ul').on('click', 'li', function() { ... });
```

### 5. How do you perform an AJAX GET request?
**A:**
```javascript
$.get('url', function(data) { ... });
```

### 6. Real-time: How do you update a table with AJAX response data?
**A:** Use a success callback to modify the DOM:
```javascript
$.get('url', function(data) {
  $('#table').html(data);
});
```

### 7. How do you chain multiple jQuery methods?
**A:**
```javascript
$('#el').addClass('active').fadeIn().text('Done');
```

### 8. Real-time: How do you prevent memory leaks in a jQuery app?
**A:** Remove event handlers with `.off()`, avoid detached DOM nodes, and clean up timers.

### 9. How do you check if an element exists before acting on it?
**A:**
```javascript
if ($('#el').length) { /* ... */ }
```

### 10. Real-time: How do you animate an element to slide up and then fade out?
**A:**
```javascript
$('#el').slideUp(400, function() {
  $(this).fadeOut();
});
```

### 11. How do you get and set the value of an input field?
**A:** Use `.val()`.

### 12. Real-time: How do you disable a button after it is clicked?
**A:**
```javascript
$('#btn').on('click', function() {
  $(this).prop('disabled', true);
});
```

### 13. How do you add and remove a class from an element?
**A:** Use `.addClass()` and `.removeClass()`.

### 14. Real-time: How do you load content from another page into a div?
**A:**
```javascript
$('#div').load('page.html');
```

### 15. How do you prevent the default action of a form submit?
**A:**
```javascript
$('form').submit(function(e) {
  e.preventDefault();
});
```

### 16. Real-time: How do you get the index of a clicked list item?
**A:**
```javascript
$('ul').on('click', 'li', function() {
  var idx = $(this).index();
});
```

### 17. How do you fade in an element?
**A:** Use `.fadeIn()`.

### 18. Real-time: How do you toggle a class on click?
**A:**
```javascript
$('#el').on('click', function() {
  $(this).toggleClass('active');
});
```

### 19. How do you get the parent of an element?
**A:** Use `.parent()`.

### 20. Real-time: How do you find all checked checkboxes in a form?
**A:**
```javascript
$('form input[type="checkbox"]:checked')
```

### 21. How do you stop an animation before it completes?
**A:** Use `.stop()`.

### 22. Real-time: How do you submit a form via AJAX?
**A:**
```javascript
$('form').submit(function(e) {
  e.preventDefault();
  $.post('url', $(this).serialize());
});
```

### 23. How do you get the value of a data attribute?
**A:** Use `.data('key')`.

### 24. Real-time: How do you remove all child elements from a div?
**A:** Use `.empty()`.

### 25. How do you check if an element has a class?
**A:** Use `.hasClass('className')`.

### 26. Real-time: How do you iterate over an array with jQuery?
**A:**
```javascript
$.each(array, function(i, val) { ... });
```

### 27. How do you merge two objects?
**A:** Use `$.extend()`.

### 28. Real-time: How do you get the text of all list items?
**A:**
```javascript
$('li').each(function() {
  console.log($(this).text());
});
```

### 29. How do you delegate an event to future elements?
**A:** Use `.on()` on a parent.

### 30. Real-time: How do you debounce a function in jQuery?
**A:** Use a timer variable to delay execution.

### 31. How do you get all siblings of an element?
**A:** Use `.siblings()`.

### 32. Real-time: How do you check if an input is empty before submitting a form?
**A:**
```javascript
if (!$('#input').val()) { alert('Input required!'); }
```

### 33. How do you clone an element?
**A:** Use `.clone()`.

### 34. Real-time: How do you animate multiple properties at once?
**A:**
```javascript
$('#box').animate({ width: '200px', height: '200px' }, 500);
```

### 35. How do you get the position of an element?
**A:** Use `.position()` or `.offset()`.

### 36. Real-time: How do you disable all inputs in a form?
**A:**
```javascript
$('form :input').prop('disabled', true);
```

### 37. How do you bind multiple events to an element?
**A:**
```javascript
$('#el').on({
  click: function() {},
  mouseenter: function() {}
});
```

### 38. Real-time: How do you get the selected value of a dropdown?
**A:**
```javascript
$('#select').val();
```

### 39. How do you remove a specific class from all elements?
**A:**
```javascript
$('.className').removeClass('className');
```

### 40. Real-time: How do you check if an AJAX request failed due to timeout?
**A:** Set `timeout` in `.ajax()` and use the `error` callback to check for `textStatus === 'timeout'`.

### 41. How do you serialize form data?
**A:** Use `.serialize()`.

### 42. Real-time: How do you get the height and width of an element?
**A:** Use `.height()` and `.width()`.

### 43. How do you stop event propagation?
**A:** Use `event.stopPropagation()` in the handler.

### 44. Real-time: How do you check if an element is visible?
**A:**
```javascript
$('#el').is(':visible');
```

### 45. How do you trigger an event programmatically?
**A:** Use `.trigger('eventName')`.

### 46. Real-time: How do you get all data attributes of an element?
**A:**
```javascript
$('#el').data();
```

### 47. How do you remove an element from the DOM?
**A:** Use `.remove()`.

### 48. Real-time: How do you check if a checkbox is checked?
**A:**
```javascript
$('#cb').is(':checked');
```

### 49. How do you delay execution of a function?
**A:** Use `setTimeout()`.

### 50. Real-time: How do you handle JSON data in an AJAX response?
**A:** Set `dataType: 'json'` in `.ajax()` and use the response in the success callback.

### 51. How do you get the index of an element among its siblings?
**A:** Use `.index()`.

### 52. Real-time: How do you prevent double form submission?
**A:** Disable the submit button on first click or use a flag variable.

### 53. How do you check if an element matches a selector?
**A:** Use `.is(selector)`.

### 54. Real-time: How do you scroll to an element smoothly?
**A:**
```javascript
$('html, body').animate({ scrollTop: $('#target').offset().top }, 500);
```

### 55. How do you get the value of a radio button group?
**A:**
```javascript
$('input[name="group"]:checked').val();
```

### 56. Real-time: How do you throttle a function in jQuery?
**A:** Use a timer to limit execution frequency.

### 57. How do you check if an element is in the viewport?
**A:** Calculate position with `.offset()` and compare to window scroll/height.

### 58. Real-time: How do you upload a file via AJAX?
**A:** Use `FormData` and set `processData: false, contentType: false` in `.ajax()`.

### 59. How do you get all checked checkboxes in a group?
**A:**
```javascript
$('input[name="group[]"]:checked')
```

### 60. Real-time: How do you dynamically load a script file?
**A:**
```javascript
$.getScript('script.js');
```

### 61. How do you check if an element is empty?
**A:** Use `.is(':empty')`.

### 62. Real-time: How do you get the scroll position of a page?
**A:**
```javascript
$(window).scrollTop();
```

### 63. How do you set multiple CSS properties at once?
**A:**
```javascript
$('#el').css({ color: 'red', background: 'yellow' });
```

### 64. Real-time: How do you detect when an image has loaded?
**A:**
```javascript
$('img').on('load', function() { /* ... */ });
```

### 65. How do you get the number of elements matching a selector?
**A:** Use `.length` property.

### 66. Real-time: How do you check if a user scrolled to the bottom of a page?
**A:** Compare `$(window).scrollTop() + $(window).height()` to `$(document).height()`.

### 67. How do you remove inline styles from an element?
**A:** Use `.removeAttr('style')`.

### 68. Real-time: How do you get the HTML content of an element?
**A:** Use `.html()`.

### 69. How do you replace one element with another?
**A:** Use `.replaceWith()`.

### 70. Real-time: How do you check if an element is hidden?
**A:**
```javascript
$('#el').is(':hidden');
```

### 71. How do you get the next all siblings of an element?
**A:** Use `.nextAll()`.

### 72. Real-time: How do you get the previous all siblings of an element?
**A:** Use `.prevAll()`.

### 73. How do you get the closest ancestor matching a selector?
**A:** Use `.closest(selector)`.

### 74. Real-time: How do you get all descendants matching a selector?
**A:** Use `.find(selector)`.

### 75. How do you check if an element contains another element?
**A:** Use `.has(selector)`.

### 76. Real-time: How do you get the outer width/height of an element (including padding and border)?
**A:** Use `.outerWidth()` and `.outerHeight()`.

### 77. How do you get the computed style of an element?
**A:** Use `.css('property')`.

### 78. Real-time: How do you trigger a custom event?
**A:**
```javascript
$('#el').trigger('myEvent');
```

### 79. How do you bind an event to multiple elements?
**A:**
```javascript
$('.btn').on('click', function() { ... });
```

### 80. Real-time: How do you get the value of a select option on change?
**A:**
```javascript
$('#select').on('change', function() {
  var val = $(this).val();
});
```

### 81. How do you check if an element is disabled?
**A:** Use `.is(':disabled')`.

### 82. Real-time: How do you get the first/last element in a set?
**A:** Use `.first()` and `.last()`.

### 83. How do you get the children of an element?
**A:** Use `.children()`.

### 84. Real-time: How do you get the parent form of an input?
**A:**
```javascript
$('#input').closest('form');
```

### 85. How do you get the data type of a variable in jQuery?
**A:** Use `$.type(variable)`.

### 86. Real-time: How do you check if a value is an array?
**A:** Use `$.isArray(value)`.

### 87. How do you extend jQuery with a custom method?
**A:** Add to `$.fn`.

### 88. Real-time: How do you get all form values as an object?
**A:** Use `.serializeArray()` and convert to object.

### 89. How do you check if an element is focusable?
**A:** Use `:focusable` selector (with jQuery UI) or custom logic.

### 90. Real-time: How do you focus an input field?
**A:**
```javascript
$('#input').focus();
```

### 91. How do you get the tag name of an element?
**A:** Use `.prop('tagName')`.

### 92. Real-time: How do you get the value of a textarea?
**A:** Use `.val()`.

### 93. How do you check if an element is selected?
**A:** Use `.is(':selected')` (for options).

### 94. Real-time: How do you get the index of a selected option?
**A:**
```javascript
$('#select option:selected').index();
```

### 95. How do you get the scroll height of an element?
**A:** Use `.prop('scrollHeight')`.

### 96. Real-time: How do you get the value of a hidden input?
**A:** Use `.val()` on the hidden input selector.

### 97. How do you check if an element is checked by default?
**A:** Use `.prop('defaultChecked')`.

### 98. Real-time: How do you get the previous sibling of an element?
**A:** Use `.prev()`.

### 99. How do you get the next sibling of an element?
**A:** Use `.next()`.

### 100. Real-time: How do you get all elements with a specific data attribute?
**A:**
```javascript
$('[data-key]');
```

## References
- [jQuery Interview Questions - GeeksforGeeks](https://www.geeksforgeeks.org/jquery-interview-questions/)
- [jQuery API](https://api.jquery.com/)
