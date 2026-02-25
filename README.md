# markdown-styles

Custom CSS for VSCode's built-in Markdown preview, served via [jsDelivr](https://www.jsdelivr.com/).

## Setup

Add this to your VSCode `settings.json`:

```json
"markdown.styles": [
  "https://cdn.jsdelivr.net/gh/petchvm/markdown-styles@main/main.css"
]
```

> VSCode's Markdown preview only loads stylesheets from whitelisted domains — raw GitHub URLs won't work, but jsDelivr does.

## What's in `main.css`

- **Inter** as the base font with OpenType features (`cv02`, `cv03`, `cv04`, `cv11`)
- Centered layout, capped at 800px
- Tighter letter-spacing on headings
- `text-wrap: pretty` for body, `balance` for headings

## Updating

1. Edit and commit the file
2. Purge the jsDelivr cache:
   ```
   https://purge.jsdelivr.net/gh/petchvm/markdown-styles@main/main.css
   ```
3. Reload the Markdown preview in VSCode
