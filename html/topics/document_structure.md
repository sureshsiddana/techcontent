# HTML Document Structure & Doctype

## Key Concepts
- **Doctype Declaration:** `<!DOCTYPE html>` tells the browser to use HTML5 and standards mode, avoiding quirks mode.
- **HTML Root Element:** `<html>` wraps the entire document and can include a `lang` attribute for language.
- **Head Section:** `<head>` contains metadata, links, scripts, styles, SEO tags, and more. Includes `<meta charset>`, `<title>`, `<link>`, `<script>`, `<meta name="viewport">` for responsive design.
- **Body Section:** `<body>` contains all visible content, including headings, paragraphs, images, forms, and scripts.
- **Character Encoding:** `<meta charset="UTF-8">` ensures proper text rendering for all languages and symbols.
- **Viewport Meta Tag:** `<meta name="viewport" content="width=device-width, initial-scale=1.0">` for mobile responsiveness.
- **Order of Elements:** Place CSS links before scripts for faster rendering.

## Real-World Example
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sample Page</title>
    <link rel="stylesheet" href="styles.css">
    <script src="main.js" defer></script>
  </head>
  <body>
    <header><h1>Hello, World!</h1></header>
    <main>
      <p>This is a sample HTML5 document structure.</p>
    </main>
    <footer>&copy; 2025 Example</footer>
  </body>
</html>
```
- Used in all web projects, emails, and web apps for consistent rendering.

## Best Practices
- Always use the HTML5 doctype.
- Set the correct language and character encoding.
- Place critical CSS in the head and defer non-essential scripts.
- Use semantic structure for accessibility and SEO.

## Interview Q&A
**Q: Why is the doctype important?**
A: It ensures the browser renders the page in standards mode, not quirks mode, for consistent cross-browser behavior.

**Q: What is the purpose of the `<head>` section?**
A: To include metadata, links to stylesheets, scripts, SEO tags, and other resources that affect the document but are not visible content.

**Q: What is the viewport meta tag for?**
A: It controls layout on mobile browsers for responsive design.

## References
- [HTML Document Structure](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/html)
- [HTML Head Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head)

## Diagram
![HTML Document Structure](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/html/html-document-structure.png)
