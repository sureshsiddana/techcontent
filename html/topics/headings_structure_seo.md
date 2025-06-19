# HTML Headings, Structure, and SEO (Advanced)

## Key Concepts
- **Heading Hierarchy:** Proper use of `<h1>` to `<h6>` for content structure and SEO.
- **Landmark Elements:** `<header>`, `<nav>`, `<main>`, `<footer>`, `<aside>` for accessibility and search engines.
- **Breadcrumbs & Structured Data:** Use of schema.org and JSON-LD for rich search results.
- **Canonical Tags:** Prevent duplicate content issues.
- **Open Graph & Twitter Cards:** Enhance sharing on social media.

## Advanced Example
```html
<header>
  <h1>HTML Advanced Structure</h1>
  <nav aria-label="Main Navigation">
    <a href="/">Home</a>
    <a href="/about">About</a>
  </nav>
</header>
<main>
  <article>
    <h2>Section Title</h2>
    <p>Content...</p>
  </article>
</main>
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [
    {"@type": "ListItem", "position": 1, "name": "Home", "item": "/"},
    {"@type": "ListItem", "position": 2, "name": "Advanced Structure", "item": "/advanced-structure"}
  ]
}
</script>
```

## Best Practices
- Use only one `<h1>` per page for the main topic.
- Use semantic elements for structure and accessibility.
- Add structured data for enhanced search results.

## Interview Q&A
**Q: How do you use structured data for SEO?**
A: Add JSON-LD or microdata to help search engines understand page content.

**Q: Why are canonical tags important?**
A: They prevent duplicate content issues and consolidate ranking signals.

## References
- [HTML SEO & Structure](https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data)
- [Open Graph Protocol](https://ogp.me/)

## Diagram
![HTML Structure for SEO](https://developers.google.com/search/docs/appearance/structured-data/html-structure-seo.png)
