# HTML Canvas & SVG

## Key Concepts
- **Canvas API:** Draw 2D graphics, charts, and animations with JavaScript.
- **SVG (Scalable Vector Graphics):** XML-based vector images, scalable without loss of quality.
- **Interactivity:** Both support dynamic updates and user interaction.
- **Accessibility:** SVG is more accessible and searchable than Canvas.
- **Performance:** Canvas is better for real-time, pixel-based graphics; SVG for static or less complex visuals.

## Advanced Example
```html
<canvas id="myCanvas" width="200" height="100"></canvas>
<script>
  const ctx = document.getElementById('myCanvas').getContext('2d');
  ctx.fillStyle = 'blue';
  ctx.fillRect(10, 10, 150, 75);
</script>
<svg width="200" height="100">
  <rect width="150" height="75" x="10" y="10" fill="green" />
</svg>
```

## Best Practices
- Use SVG for icons, logos, and static graphics.
- Use Canvas for games, visualizations, and real-time drawing.

## Interview Q&A
**Q: When should you use Canvas over SVG?**
A: Use Canvas for complex, real-time, or pixel-based graphics; SVG for static, scalable images.

**Q: How do you make SVG graphics accessible?**
A: Use `title`, `desc`, and ARIA attributes.

## References
- [Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [SVG Guide](https://developer.mozilla.org/en-US/docs/Web/SVG)

## Diagram
![Canvas vs SVG](https://developer.mozilla.org/en-US/docs/Web/SVG/canvas-vs-svg.png)
