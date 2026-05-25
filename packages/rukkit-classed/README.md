# Rukkit Classed — Utility Classes Flavor

> One warm, editorial CSS library. Explicit `.rk-*` utilities, complete control.

**Rukkit Classed** provides explicit `.rk-*` utility classes for styling. Use semantic HTML with targeted class selectors for maximum control. ~18 KB gzipped, zero JavaScript, five complete design directions.

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit-classed@1/dist/rukkit.css">
<body>
  <div class="rk-container">
    <h1 class="rk-heading-1">Hello, Rukkit</h1>
    <button class="rk-button rk-button-primary">Click me</button>
  </div>
</body>
```

---

## Install

### CDN (jsDelivr) — Recommended

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit-classed@1/dist/rukkit.css">
```

### unpkg

```html
<link rel="stylesheet" href="https://unpkg.com/rukkit-classed@1/dist/rukkit.css">
```

Pin to a specific version:

```html
<link rel="stylesheet" href="https://unpkg.com/rukkit-classed@1.0.0/dist/rukkit.css">
```

### npm / yarn / pnpm

```bash
npm install rukkit-classed
yarn add rukkit-classed
pnpm add rukkit-classed
```

Import in your bundler:

```js
import 'rukkit-classed';
```

Or import the CSS directly:

```js
import 'rukkit-classed/dist/rukkit.css';
```

### Download

```bash
curl -O https://unpkg.com/rukkit-classed/dist/rukkit.css
```

Or grab `dist/rukkit.css` from the GitHub repository.

---

## Two Flavors

Choose your flavor:

- **[Rukkit](https://www.npmjs.com/package/rukkit)** — Classless. Just semantic HTML.
- **Rukkit Classed** (this package) — Explicit `.rk-*` utility classes.

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
  
  <!-- Rukkit Classed -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit-classed@1/dist/rukkit.css">
  
  <!-- Optional: Google Fonts (recommended for best typography) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;450;500;600&family=JetBrains+Mono:wght@400;500;600&family=Fraunces:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>
  <main class="rk-container">
    <article>
      <h1 class="rk-heading-1">Welcome to Rukkit</h1>
      <p class="rk-text">Write semantic HTML with explicit classes.</p>
    </article>
  </main>
</body>
</html>
```

### 2. Use utility classes

Rukkit Classed provides explicit `.rk-*` classes:

```html
<!-- Typography -->
<h1 class="rk-heading-1">Heading 1</h1>
<h2 class="rk-heading-2">Heading 2</h2>
<p class="rk-text">Paragraph text</p>
<p class="rk-text-muted">Muted text</p>

<!-- Buttons -->
<button class="rk-button">Default</button>
<button class="rk-button rk-button-primary">Primary</button>
<button class="rk-button rk-button-secondary">Secondary</button>
<button class="rk-button" disabled>Disabled</button>

<!-- Forms -->
<form class="rk-form">
  <label class="rk-label">Email
    <input type="email" class="rk-input" placeholder="you@example.com">
  </label>
  <button type="submit" class="rk-button rk-button-primary">Submit</button>
</form>

<!-- Containers & Layout -->
<div class="rk-container">
  <div class="rk-grid rk-grid-2">
    <div class="rk-card">Card 1</div>
    <div class="rk-card">Card 2</div>
  </div>
</div>

<!-- Code -->
<code class="rk-code">const hello = "world";</code>
<pre class="rk-pre"><code>function greet() {
  console.log("Hello!");
}</code></pre>
```

---

## Available Classes

### Typography

- `.rk-heading-1` — Large headline
- `.rk-heading-2` — Secondary headline
- `.rk-heading-3` — Tertiary headline
- `.rk-text` — Body text
- `.rk-text-muted` — Secondary text
- `.rk-text-small` — Small text
- `.rk-text-lead` — Lead paragraph

### Buttons

- `.rk-button` — Base button
- `.rk-button-primary` — Primary action
- `.rk-button-secondary` — Secondary action
- `.rk-button-small` — Small button
- `.rk-button-large` — Large button

### Forms

- `.rk-form` — Form container
- `.rk-input` — Text input
- `.rk-textarea` — Textarea
- `.rk-select` — Select dropdown
- `.rk-label` — Form label
- `.rk-help-text` — Help text below inputs

### Layout

- `.rk-container` — Centered content container
- `.rk-grid` — Grid layout
- `.rk-grid-2` — Two-column grid
- `.rk-grid-3` — Three-column grid
- `.rk-grid-4` — Four-column grid

### Components

- `.rk-card` — Card component
- `.rk-card-header` — Card header
- `.rk-card-body` — Card body
- `.rk-card-footer` — Card footer

### Code

- `.rk-code` — Inline code
- `.rk-pre` — Code block

---

## What's Included

- ✅ Comprehensive utility classes
- ✅ Beautiful typography (Inter, JetBrains Mono, Fraunces)
- ✅ Form elements (inputs, buttons, textareas, selects)
- ✅ Code blocks and syntax-friendly pre/code
- ✅ Tables with clean, readable styling
- ✅ Cards and layout components
- ✅ Media queries for responsive design
- ✅ Dark mode support via CSS custom properties
- ✅ Five design directions (configurable via tokens)
- ✅ Zero JavaScript dependencies

---

## Theming with Tokens

Override CSS custom properties for easy customization:

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
rukkit-classed/
├── dist/
│   └── rukkit.css          # Compiled, minified stylesheet
├── src/
│   ├── _tokens.css         # Design tokens and variables
│   ├── _reset.css          # CSS reset
│   ├── _typography.css     # Typography classes
│   ├── _buttons.css        # Button classes
│   ├── _forms.css          # Form classes
│   ├── _layout.css         # Layout and grid classes
│   ├── _components.css     # Card and component classes
│   ├── _utilities.css      # Utility classes
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
cd rukkit/packages/rukkit-classed

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

- [Rukkit](https://www.npmjs.com/package/rukkit) — Classless flavor
- [Design System Tokens](https://github.com/yourusername/rukkit)
- [Live Examples](https://rukkit.design)
