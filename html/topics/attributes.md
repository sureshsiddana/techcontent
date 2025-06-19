# HTML Attributes

## Key Concepts
- **Attributes:** Provide additional information about elements (e.g., `class`, `id`, `src`, `href`). Placed inside the opening tag.
- **Global Attributes:** Can be used on any element (e.g., `title`, `style`, `data-*`, `tabindex`, `hidden`, `draggable`).
- **Boolean Attributes:** Attributes that are either present or not (e.g., `checked`, `disabled`, `readonly`, `required`).
- **Data Attributes:** Custom attributes prefixed with `data-` for storing extra information (e.g., `<div data-user-id="123">`).
- **ARIA Attributes:** Improve accessibility for users with disabilities (e.g., `aria-label`, `aria-hidden`).
- **Event Attributes:** Inline event handlers (e.g., `onclick`, `onchange`)—not recommended for modern development.

## Real-World Example
- Using `class` and `id` for CSS styling and JavaScript targeting.
```html
<button id="submitBtn" class="btn primary" data-action="save" aria-label="Save">Save</button>
```
- Using `tabindex` for keyboard navigation:
```html
<a href="#" tabindex="0">Focusable Link</a>
```

## Best Practices
- Use `id` only for unique elements; use `class` for reusable styles.
- Prefer external JS event listeners over inline event attributes.
- Use ARIA and data attributes for accessibility and custom data.

## Interview Q&A
**Q: What is the difference between `id` and `class`?**
A: `id` is unique per page and used for single elements; `class` can be used on multiple elements for styling or scripting.

**Q: What are data attributes?**
A: Custom attributes prefixed with `data-` for storing extra information, accessible via JavaScript (e.g., `element.dataset.userId`).

**Q: What are ARIA attributes?**
A: Attributes that improve accessibility for users with assistive technologies.

## References
- [HTML Attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)
- [ARIA Reference](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes)

## Relevant Image
![HTML Attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/html-attributes.png)
