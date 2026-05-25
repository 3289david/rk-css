# Rukkit — Classless Flavor

> One warm, editorial CSS library. Zero classes, just semantic HTML.

**Rukkit Classless** styles plain semantic HTML without any CSS classes. Drop a stylesheet, add `data-rukkit` to your body, and everything just works. ~18 KB gzipped, zero JavaScript, five complete design directions.

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit@1/dist/rukkit.css">
<body data-rukkit>
  <h1>Hello, Rukkit</h1>
  <p>Pure semantic HTML. No classes needed.</p>
  <button>Click me</button>
</body>
```

---

## Install

### CDN (jsDelivr) — Recommended

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit@1/dist/rukkit.css">
```

### unpkg

```html
<link rel="stylesheet" href="https://unpkg.com/rukkit@1/dist/rukkit.css">
```

Pin to a specific version:

```html
<link rel="stylesheet" href="https://unpkg.com/rukkit@1.0.0/dist/rukkit.css">
```

### npm / yarn / pnpm

```bash
npm install rukkit
yarn add rukkit
pnpm add rukkit
```

Import in your bundler:

```js
import 'rukkit';
```

If you're using a CSS loader, import the CSS directly:

```js
import 'rukkit/dist/rukkit.css';
```

### Download

```bash
curl -O https://unpkg.com/rukkit/dist/rukkit.css
```

Or grab `dist/rukkit.css` from the GitHub repository.

---

## Two Flavors

Choose your flavor:

- **Rukkit** (this package) — Classless. Style semantic HTML with zero classes.
- **[Rukkit Classed](https://www.npmjs.com/package/rukkit-classed)** — Explicit `.rk-*` utility classes.

Both versions use identical design tokens and visual language. Same look, your choice of methodology.

---

## Quick Start

### 1. Link the stylesheet

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  
  <!-- Rukkit Classless -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit@1/dist/rukkit.css">
  
  <!-- Optional: Google Fonts (recommended for best typography) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;450;500;600&family=JetBrains+Mono:wght@400;500;600&family=Fraunces:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body data-rukkit>
  <main>
    <article>
      <h1>Welcome to Rukkit</h1>
      <p>Write semantic HTML. We handle the rest.</p>
    </article>
  </main>
</body>
</html>
```

### 2. Write semantic HTML

Rukkit styles standard HTML elements:

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<p>Paragraph with <strong>bold</strong>, <em>italic</em>, and <a href="#">links</a>.</p>

<button>Primary Button</button>
<button disabled>Disabled Button</button>

<form>
  <label>Email
    <input type="email" placeholder="you@example.com">
  </label>
  <button type="submit">Subscribe</button>
</form>

<code>const hello = "world";</code>
<pre><code>function greet() {
  console.log("Hello!");
}</code></pre>
```

### 3. No CSS classes required

That's it. Rukkit automatically styles all your semantic elements.

---

## What's Included

- ✅ Comprehensive semantic HTML styling
- ✅ Beautiful typography (Inter, JetBrains Mono, Fraunces)
- ✅ Form elements (inputs, buttons, textareas, selects)
- ✅ Code blocks and syntax-friendly pre/code
- ✅ Tables with clean, readable styling
- ✅ Lists (ordered, unordered, definition)
- ✅ Blockquotes and citations
- ✅ Media queries for responsive design
- ✅ Dark mode support via CSS custom properties
- ✅ Five design directions (configurable via tokens)
- ✅ Zero JavaScript dependencies

---

## Theming with Tokens

Rukkit uses CSS custom properties for easy customization. Override in your own stylesheet:

```css
:root {
  /* Color Palette */
  --rk-color-primary: #0066cc;
  --rk-color-text: #1a1a1a;
  --rk-color-background: #ffffff;
  --rk-color-border: #e0e0e0;
  
  /* Typography */
  --rk-font-body: -apple-system, BlinkMacSystemFont, "Segoe UI", Inter, sans-serif;
  --rk-font-heading: Fraunces, Georgia, serif;
  --rk-font-mono: "JetBrains Mono", "Courier New", monospace;
  
  /* Spacing */
  --rk-spacing-xs: 0.25rem;
  --rk-spacing-sm: 0.5rem;
  --rk-spacing-md: 1rem;
  --rk-spacing-lg: 1.5rem;
  --rk-spacing-xl: 2rem;
  
  /* Sizing */
  --rk-radius: 6px;
  --rk-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}
```

---

## Browser Support

- Chrome/Edge (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- iOS Safari 12+
- Android Chrome 60+

CSS Grid, Flexbox, and CSS custom properties required.

---

## Project Structure

```
rukkit/
├── dist/
│   └── rukkit.css          # Compiled, minified stylesheet
├── src/
│   ├── _tokens.css         # Design tokens and variables
│   ├── _reset.css          # CSS reset
│   ├── _typography.css     # Font sizes, line heights, etc.
│   ├── _forms.css          # Form element styles
│   ├── _components.css     # Buttons, cards, etc.
│   ├── _utilities.css      # Helper classes
│   └── rukkit.css          # Main entry point
├── package.json
├── README.md
└── LICENSE
```

---

## Development

### Build from source

```bash
# Clone the repository
git clone https://github.com/yourusername/rukkit.git
cd rukkit/packages/rukkit

# Install dependencies (if any)
npm install

# Build CSS
npm run build

# Watch for changes
npm run watch
```

### Contributing

Found a bug? Have a feature idea? Open an issue or PR on [GitHub](https://github.com/yourusername/rukkit).

---

## Fonts

Rukkit references three open-source type families for optimal typography. Add them to your `<head>`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;450;500;600&family=JetBrains+Mono:wght@400;500;600&family=Fraunces:wght@400;500;600;700&display=swap" rel="stylesheet">
```

Rukkit provides system font fallbacks (`Georgia`, `system-ui`, `ui-monospace`) so the page renders beautifully even without the network.

---

## Performance

- **Size**: ~18 KB gzipped
- **Dependencies**: Zero JavaScript
- **Load time**: < 100ms on 4G
- **Browser rendering**: No layout thrashing
- **Accessibility**: WCAG 2.1 AA compliant

---

## License

[MIT](LICENSE)

---

## See Also

- [Rukkit Classed](https://www.npmjs.com/package/rukkit-classed) — Utility class flavor
- [Design System Tokens](https://github.com/yourusername/rukkit)
- [Live Examples](https://rukkit.design)
