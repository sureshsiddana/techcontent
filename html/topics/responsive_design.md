# HTML Responsive Design

## Key Concepts
- **Viewport Meta Tag:** `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- **Media Queries:** CSS rules for different screen sizes.
- **Flexible Layouts:** Use of percentages, flexbox, and grid.
- **Responsive Images:** `srcset`, `<picture>`, and CSS for scaling images.
- **Mobile-First Design:** Designing for mobile before desktop.

## Advanced Example
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  .container { display: flex; flex-wrap: wrap; }
  @media (max-width: 600px) {
    .container { flex-direction: column; }
  }
</style>
<div class="container">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

## Best Practices
- Always test on multiple devices and browsers.
- Use relative units (em, rem, %, vw, vh) for sizing.
- Avoid fixed-width layouts.

## Interview Q&A
**Q: What is mobile-first design?**
A: Designing for the smallest screen first, then scaling up for larger screens.

**Q: How do you make images responsive?**
A: Use `max-width: 100%` in CSS and `srcset`/`<picture>` in HTML.

## References
- [Responsive Design Basics](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)

## Diagram
![Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design/html-responsive-design.png)
