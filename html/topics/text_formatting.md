# HTML Text Formatting

## Key Concepts
- **Headings:** `<h1>` to `<h6>` for content hierarchy. Use only one `<h1>` per page for SEO.
- **Paragraphs:** `<p>` for blocks of text. Browsers add margin above and below by default.
- **Bold & Italic:** `<b>`, `<strong>` for bold; `<i>`, `<em>` for italics. Use `<strong>` and `<em>` for semantic emphasis (important for accessibility and SEO).
- **Line Breaks & Horizontal Rules:** `<br>` for line breaks, `<hr>` for thematic breaks or section dividers.
- **Preformatted Text:** `<pre>` preserves whitespace, tabs, and line breaks. Useful for code snippets.
- **Quotations:** `<blockquote>` for long quotes (with optional `cite`), `<q>` for short inline quotes, `<cite>` for references.
- **Lists:** Use `<ul>`, `<ol>`, `<li>` for structured text (see dedicated topic).
- **Special Characters:** Use HTML entities (e.g., `&amp;`, `&lt;`, `&copy;`) for reserved symbols.

## Real-World Example
```html
<h1>Welcome</h1>
<p>This is a <strong>sample</strong> paragraph with <em>emphasis</em> and a <a href="#">link</a>.</p>
<blockquote cite="https://example.com">This is a blockquote.</blockquote>
<pre><code>function hello() {
  return 'Hello, world!';
}</code></pre>
```
- Formatting is crucial for readability, accessibility, and SEO.

## Best Practices
- Use semantic tags for meaning, not just appearance.
- Avoid excessive use of `<br>` for layout—use CSS for spacing.
- Use `<strong>` and `<em>` for important content, not just for styling.
- Always escape special characters in code and user input.

## Interview Q&A
**Q: What is the difference between `<b>` and `<strong>`?**
A: `<b>` is purely visual; `<strong>` indicates importance for accessibility/SEO.

**Q: How do you preserve whitespace in HTML?**
A: Use the `<pre>` tag.

**Q: Why use semantic tags for formatting?**
A: They improve accessibility, SEO, and make your code easier to maintain.

## References
- [HTML Text Fundamentals](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p)
- [HTML Entities](https://developer.mozilla.org/en-US/docs/Glossary/Entity)

## Diagram
![HTML Text Formatting](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p/html-text-formatting.png)
