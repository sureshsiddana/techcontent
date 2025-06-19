# HTML Audio & Video

## Key Concepts
- **<audio> and <video> Tags:** Embed media with native controls.
- **Attributes:** `controls`, `autoplay`, `loop`, `muted`, `preload`, `poster` (for video).
- **Multiple Sources:** `<source>` for fallback formats.
- **Captions & Subtitles:** `<track>` for accessibility.
- **Streaming & Adaptive Bitrate:** HLS, DASH for advanced video delivery.

## Advanced Example
```html
<video controls width="400" poster="preview.jpg">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  <track kind="captions" src="captions_en.vtt" srclang="en" label="English">
  Sorry, your browser doesn't support embedded videos.
</video>
```

## Best Practices
- Always provide captions for accessibility.
- Use multiple formats for broad browser support.
- Optimize media files for web delivery.

## Interview Q&A
**Q: How do you add subtitles to a video in HTML?**
A: Use the `<track>` element with kind="captions" or kind="subtitles".

**Q: What is adaptive bitrate streaming?**
A: Serving different video qualities based on user bandwidth.

## References
- [HTML Video](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)
- [HTML Audio](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio)

## Diagram
![HTML Video Tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video/html-video-tag.png)
