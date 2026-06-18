# CLAUDE.md

## Project Overview

This is a **single-page personal portfolio/resume website** written in Chinese. It consists of a single `index.html` file with all styles embedded in a `<style>` block — no build tools, no JavaScript frameworks, no external dependencies.

## Tech Stack

- **HTML5** — semantic markup, Chinese (`zh-CN`) language
- **CSS3** — embedded in `<style>`, uses gradients, flexbox, grid, and responsive media queries
- **No JavaScript** — the page is purely static
- **No build system** — open `index.html` directly in a browser to preview

## File Structure

```
index.html   # The entire application — markup + styles in one file
```

## Development

- **Preview:** Open `index.html` in any modern browser. No server required.
- **Editing:** All changes go into `index.html`. Keep styles in the existing `<style>` block and markup in the `<body>`.

## Code Style & Conventions

- CSS selectors use class names (`.card`, `.section-title`, `.skill-tag`, etc.)
- Utility classes for icons use short prefixes (`.ci-email`, `.ci-phone`, etc.)
- Emojis are used as icons — no icon library
- Responsive breakpoint is at `500px` (single `@media` rule at the bottom of the `<style>` block)
- Colors follow a purple/indigo gradient theme (`#667eea`, `#764ba2`, `#6c5ce7`, `#a29bfe`)

## Guidelines for Claude

1. **Keep it simple** — this is a single-file static page. Don't introduce build tools, frameworks, or additional files unless explicitly asked.
2. **Preserve the Chinese content** — all user-facing text is in Chinese. Maintain that when editing placeholder content.
3. **Respect the design system** — stick to the existing color palette, card layout, and gradient theme. When adding new sections, reuse existing class patterns (`.section`, `.section-title`, `.timeline-item`, etc.).
4. **Mobile-first awareness** — any new layout should work at narrow widths. The existing `@media (max-width: 500px)` rule is the only breakpoint.
5. **No external dependencies** — don't add CDN links, external fonts, or third-party scripts unless explicitly requested.
6. **Keep everything in one file** — markup, styles, and any future scripts all belong in `index.html`.
