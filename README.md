# Rukkit UI

> One warm, editorial CSS library. **Two independent packages** — choose your flavor.

Rukkit is an opinionated, production-ready CSS framework with two distinct flavors:

- **[Rukkit](https://www.npmjs.com/package/rukkit)** — Classless. Styles plain semantic HTML with zero CSS classes.
- **[Rukkit Classed](https://www.npmjs.com/package/rukkit-classed)** — Utility classes. Explicit `.rk-*` classes for maximum control.

Both packages use **identical design tokens and visual language**. ~18 KB gzipped, zero JavaScript dependencies, five complete design directions, and production-ready out of the box.

---

## Quick Comparison

| Feature | Rukkit (Classless) | Rukkit Classed |
|---------|-------------------|-----------------|
| **HTML** | Semantic only | Semantic + classes |
| **Learning curve** | Minimal | Minimal |
| **Class usage** | None | `.rk-*` utilities |
| **Use case** | Content-heavy sites, blogs | Component-heavy applications |
| **Customization** | CSS custom properties | CSS custom properties |
| **Size** | ~18 KB gzipped | ~18 KB gzipped |
| **Browser support** | Modern browsers | Modern browsers |

---

## Install

### Rukkit (Classless)

```bash
npm install rukkit
yarn add rukkit
pnpm add rukkit
```

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit@1/dist/rukkit.css">
```

### Rukkit Classed

```bash
npm install rukkit-classed
yarn add rukkit-classed
pnpm add rukkit-classed
```

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit-classed@1/dist/rukkit.css">
```

---

## Quick Start

### Rukkit (Classless) — Just use semantic HTML

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit@1/dist/rukkit.css">
</head>
<body data-rukkit>
  <main>
    <h1>Hello, Rukkit</h1>
    <p>Pure semantic HTML. Everything is styled by default.</p>
    <button>Click me</button>
  </main>
</body>
</html>
```

### Rukkit Classed — Use explicit classes

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit-classed@1/dist/rukkit.css">
</head>
<body>
  <main class="rk-container">
    <h1 class="rk-heading-1">Hello, Rukkit</h1>
    <p class="rk-text">Use explicit classes for fine-grained control.</p>
    <button class="rk-button rk-button-primary">Click me</button>
  </main>
</body>
</html>
```

---

## Package Details

### Rukkit

[Full documentation →](https://www.npmjs.com/package/rukkit)

- **NPM**: [`rukkit`](https://www.npmjs.com/package/rukkit)
- **Size**: ~18 KB gzipped
- **Ideal for**: Blogs, documentation, content-heavy sites
- **Method**: Semantic HTML styling (no classes required)

```js
import 'rukkit';
```

### Rukkit Classed

[Full documentation →](https://www.npmjs.com/package/rukkit-classed)

- **NPM**: [`rukkit-classed`](https://www.npmjs.com/package/rukkit-classed)
- **Size**: ~18 KB gzipped
- **Ideal for**: Applications, component libraries, custom layouts
- **Method**: Explicit `.rk-*` utility classes

```js
import 'rukkit-classed';
```

---

## Features

Both packages include:

✅ **Comprehensive HTML styling** — All semantic elements styled beautifully
✅ **Professional typography** — Inter, Fraunces, JetBrains Mono
✅ **Form elements** — Inputs, buttons, textareas, selects, and more
✅ **Code styling** — Inline code, code blocks, syntax-friendly
✅ **Tables** — Clean, readable table styling
✅ **Lists** — Ordered, unordered, and definition lists
✅ **Responsive design** — Mobile-first, works everywhere
✅ **Dark mode** — Built-in support via CSS variables
✅ **Design tokens** — Fully customizable via CSS custom properties
✅ **Production ready** — Battle-tested, zero dependencies

---

## Theming

Both flavors use identical CSS custom properties for customization:

```css
:root {
  /* Colors */
  --rk-color-primary: #0066cc;
  --rk-color-text: #1a1a1a;
  --rk-color-background: #ffffff;
  --rk-color-border: #e0e0e0;
  
  /* Typography */
  --rk-font-body: -apple-system, BlinkMacSystemFont, "Segoe UI", Inter, sans-serif;
  --rk-font-heading: Fraunces, Georgia, serif;
  --rk-font-mono: "JetBrains Mono", "Courier New", monospace;
  
  /* Spacing scale */
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

- ✅ Chrome/Edge (latest 2 versions)
- ✅ Firefox (latest 2 versions)
- ✅ Safari (latest 2 versions)
- ✅ iOS Safari 12+
- ✅ Android Chrome 60+

Requires CSS Grid, Flexbox, and CSS custom properties support.

---

## Performance

| Metric | Value |
|--------|-------|
| **Gzipped size** | ~18 KB |
| **Uncompressed** | ~60 KB |
| **JavaScript** | 0 bytes |
| **Dependencies** | None |
| **Load time** | < 100ms (4G) |
| **Paint time** | < 50ms |

---

## Fonts

Both packages reference three open-source typefaces. Add them to your `<head>`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;450;500;600&family=JetBrains+Mono:wght@400;500;600&family=Fraunces:wght@400;500;600;700&display=swap" rel="stylesheet">
```

System font fallbacks ensure beautiful rendering even without the network.

---

## CDN Options

### jsDelivr (Recommended)

```html
<!-- Classless -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit@1/dist/rukkit.css">

<!-- Classed -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit-classed@1/dist/rukkit.css">
```

### unpkg

```html
<!-- Classless -->
<link rel="stylesheet" href="https://unpkg.com/rukkit@1/dist/rukkit.css">

<!-- Classed -->
<link rel="stylesheet" href="https://unpkg.com/rukkit-classed@1/dist/rukkit.css">
```

---

## Project Structure

```
rukkit/
├── packages/
│   ├── rukkit/                 # Classless flavor
│   │   ├── dist/
│   │   │   └── rukkit.css
│   │   ├── src/
│   │   ├── package.json
│   │   └── README.md
│   └── rukkit-classed/         # Classed flavor
│       ├── dist/
│       │   └── rukkit.css
│       ├── src/
│       ├── package.json
│       └── README.md
├── css/                        # Source CSS files
│   ├── rukkit.css
│   └── rukkit.classed.css
├── index.html                  # Demo page
├── README.md                   # This file
└── LICENSE
```

---

## Development

### Setup

```bash
git clone https://github.com/yourusername/rukkit.git
cd rukkit
npm install
```

### Build

```bash
# Build both packages
npm run build

# Watch for changes
npm run watch
```

### Contributing

Found a bug? Have an idea? Open an issue or pull request on [GitHub](https://github.com/yourusername/rukkit).

---

## License

[MIT](LICENSE) — Free for commercial and personal use.

---

## Two flavors

### Classless

`css/rukkit.css` styles semantic HTML directly. Add `data-rukkit` to a scope and write plain markup:

```html
<body data-rukkit>
  <main>
    <h1>The quiet revolution.</h1>
    <p>Style first, structure second, scripts last.</p>
    <button>Get started</button>
    <button type="reset">Cancel</button>
  </main>
</body>
```

Variants come from semantic attributes, not class names:

| Element | Default | Variant |
|---|---|---|
| `<button>` | Ink pill (primary) | `type="submit"` → indigo, `type="reset"` → ghost outline |
| `<input>` | Soft rectangle | `type="search"` → pill shape |
| `<a>` | Underlined indigo link | `role="button"` → ghost button styling |
| `<h5>` | Eyebrow with signal dot | `<h6>` → eyebrow without dot |

Use `data-rukkit-skip` on any node to opt out of styling within the scope:

```html
<body data-rukkit>
  <article>This gets styled.</article>
  <div data-rukkit-skip>This does not.</div>
</body>
```

### Classed

`css/rukkit.classed.css` exposes explicit utilities. Use it when you need named variants and predictable class hooks:

```html
<article class="rk-card rk-card--cream">
  <p class="rk-eyebrow">Featured</p>
  <h3 class="rk-subhead">Hello, Rukkit</h3>
  <p class="rk-body">A card with explicit variant control.</p>
  <button class="rk-btn rk-btn--primary">Open →</button>
  <button class="rk-btn rk-btn--ghost">Cancel</button>
</article>
```

### Use both

The classless rules are scoped to `[data-rukkit]`. The classed rules use a `.rk-*` prefix. They never collide — you can mix them freely.

---

## Quick start

The shortest possible example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My page</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/rukkit-css@1/dist/rukkit.css">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;450;500;600&family=JetBrains+Mono:wght@400;500;600&family=Fraunces:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body data-rukkit>
  <main>
    <h5>v1.0 · ready</h5>
    <h1>Hello, Rukkit.</h1>
    <p>Drop in semantic HTML and watch it become a finished page.</p>
    <button type="submit">Get started →</button>
    <button type="reset">Maybe later</button>
  </main>
</body>
</html>
```

Open it in a browser. That's it.

---

## What's included

Every element below is styled out of the box. No classes needed.

### Typography
- `<h1>`–`<h6>` — display ladder with negative letter-spacing
- `<p>`, `<small>`, `<strong>`, `<em>`, `<a>`, `<mark>`
- `<blockquote>` + `<cite>` — editorial pull-quote
- `<code>`, `<kbd>`, `<samp>`, `<pre>` — monospace family

### Layout
- `<main>` — centered max-width container
- `<section>` — generous vertical padding
- `<article>` — surface card with hairline border
- `<aside>` — cream-filled card
- `<figure>` + `<figcaption>` — image with caption
- `<header>`, `<footer>`, `<hr>`

### Forms
- `<input>` (text, email, password, search, tel, url, number, date, time)
- `<textarea>`, `<select>`
- `<button>` (ink default, `type=submit` indigo, `type=reset` ghost)
- `<input type="checkbox">`, `<input type="radio">` — custom-painted
- `<progress>`, `<meter>` — pill-shaped bars
- `<fieldset>`, `<legend>`, `<label>`

### Lists & tables
- `<ul>` — ASCII bracket markers (`[+]`)
- `<ol>` — tabular leading zeros
- `<dl>` / `<dt>` / `<dd>` — definition-list grid
- `<table>` — tabular-numeric last column, dashboard-style header

### Native components
- `<details>` + `<summary>` — accordion with +/− toggle
- `<dialog>` — modal with backdrop blur
- `<nav>` — floating pill nav

### Inline
- Selection color, focus rings, image rounding, video chrome

---

## Theming with tokens

Every value is a CSS custom property. Override on `:root` (or any scope) to retheme.

```css
:root {
  /* Fonts */
  --rk-font-display: "Fraunces", Georgia, serif;
  --rk-font-body:    "Inter", system-ui, sans-serif;
  --rk-font-mono:    "JetBrains Mono", monospace;

  /* Surfaces */
  --rk-canvas:       #f4f0e6;   /* warm cream */
  --rk-surface:      #fbf8f1;   /* lifted cream */
  --rk-ink:          #1a1714;   /* warm near-black */

  /* Accent */
  --rk-accent:       #3a3aef;   /* indigo */
  --rk-signal:       #cf4500;   /* burnt orange */

  /* Radii */
  --rk-r-sm:         6px;
  --rk-r-md:         16px;
  --rk-r-lg:         24px;
  --rk-r-pill:       9999px;
}
```

### Dark mode

Wrap your overrides in a media query:

```css
@media (prefers-color-scheme: dark) {
  :root {
    --rk-canvas:  #1a1714;
    --rk-surface: #2a2520;
    --rk-ink:     #f4f0e6;
    --rk-paper:   #2a2520;
  }
}
```

A first-party dark theme ships in v1.2.

### Scoped themes

Apply a different palette to one region:

```html
<section style="--rk-accent: #cf4500; --rk-canvas: #fff;">
  <button type="submit">Burnt orange in here</button>
</section>
```

### Full token reference

| Token | Default | Purpose |
|---|---|---|
| `--rk-canvas` | `#f4f0e6` | Page background |
| `--rk-surface` | `#fbf8f1` | Card / lifted background |
| `--rk-cream` | `#ece6d4` | Cream interlude |
| `--rk-paper` | `#ffffff` | Pure-white inputs |
| `--rk-ink` | `#1a1714` | Text + dark surfaces |
| `--rk-muted` | `rgba(26,23,20,0.62)` | Secondary text |
| `--rk-accent` | `#3a3aef` | Primary action |
| `--rk-signal` | `#cf4500` | Highlight / emphasis |
| `--rk-signal-warm` | `#f37338` | Eyebrow dot, accents |
| `--rk-border` | `rgba(26,23,20,0.10)` | Hairline borders |
| `--rk-r-sm` | `6px` | Inputs, small radii |
| `--rk-r-md` | `16px` | Cards |
| `--rk-r-lg` | `24px` | Large cards |
| `--rk-r-xl` | `40px` | Hero containers |
| `--rk-r-pill` | `9999px` | Buttons, nav, search |
| `--rk-shadow-inset` | _multi-layer_ | Button inset shadow |
| `--rk-focus-ring` | `0 0 0 3px rgba(58,58,239,0.22)` | Focus halo |

---

## Browser support

Modern evergreen browsers. The library uses:

- CSS custom properties (broadly supported since 2017)
- `color-mix()` for hover states (Chrome 111+, Safari 16.2+, Firefox 113+)
- `:has()` for a few interactions (Chrome 105+, Safari 15.4+, Firefox 121+)
- `backdrop-filter` on the floating nav (with `-webkit-` fallback)

Graceful degradation on older browsers: layout still works; hover/focus states fall back to simpler styles.

---

## Project structure

```
rukkit/
├── css/
│   ├── rukkit.css            # classless (~18 KB)
│   └── rukkit.classed.css    # classed (~16 KB)
├── index.html                # interactive playground
└── README.md
```

The playground at `index.html` includes:

- A live HTML sandbox (edit on the left, render on the right)
- Side-by-side classless vs. classed examples
- A live theme tweaker (bottom-right, or press <kbd>T</kbd>) for accent, canvas, radii, and base font size
- Scroll-spy navigation, reveal-on-scroll, copy-to-clipboard, and a working `<dialog>` demo

---

## Inspirations

Rukkit synthesizes the best ideas from five great design traditions:

- **Reverent product presentation** — quiet, photography-first minimalism
- **Humanist warmth** — opacity-derived neutrals and inset-shadow buttons
- **Editorial gravity** — extreme radii, circular portrait cards, orbital motifs
- **Terminal aesthetics** — monospace meta, ASCII bracket markers, one dark moment
- **Atmospheric gradients** — thin-weight display tracking, tabular financial data

None of those traditions belong to anyone in particular; the principles do. Rukkit is original work — original colors, original radii, original components — informed by the spirit of those systems but not a copy of any of them.

---

## License

MIT © 2026 — do whatever you want with it.

---

## Contributing

Issues, PRs, and design suggestions welcome. The library lives in two short CSS files; nothing is hidden.

```bash
git clone https://github.com/example/rukkit-css
cd rukkit-css
# open index.html in a browser — that's the dev environment
```
