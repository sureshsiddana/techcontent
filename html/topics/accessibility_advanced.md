# HTML Accessibility: Advanced Techniques

## Key Concepts
- **ARIA Landmarks & Roles:** Use `role` attributes for custom widgets.
- **Keyboard Navigation:** Ensure all interactive elements are accessible via keyboard (tab, enter, space, arrow keys).
- **Focus Management:** Use `tabindex`, `aria-activedescendant`, and JavaScript to manage focus.
- **Screen Reader Testing:** Use NVDA, JAWS, or VoiceOver to test accessibility.
- **Accessible Modals & Dialogs:** Trap focus, provide escape, and announce with ARIA.

## Advanced Example
```html
<button aria-haspopup="dialog" aria-controls="modal1">Open Modal</button>
<div id="modal1" role="dialog" aria-modal="true" aria-labelledby="modalTitle" tabindex="-1" hidden>
  <h2 id="modalTitle">Modal Title</h2>
  <button aria-label="Close" onclick="closeModal()">&times;</button>
  <p>Modal content...</p>
</div>
```

## Best Practices
- Test with multiple assistive technologies.
- Use ARIA only when native HTML is insufficient.
- Provide skip links and visible focus indicators.

## Interview Q&A
**Q: How do you make a custom dropdown accessible?**
A: Use ARIA roles, keyboard navigation, and manage focus programmatically.

**Q: What is the purpose of `aria-live`?**
A: Announces dynamic content changes to screen readers.

## References
- [WAI-ARIA Authoring Practices](https://www.w3.org/WAI/ARIA/apg/)
- [Accessibility Testing Tools](https://www.w3.org/WAI/test-evaluate/)

## Diagram
![HTML Accessibility Advanced](https://www.w3.org/WAI/ARIA/apg/img/aria-accessibility-advanced.png)
