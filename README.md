# markdown-styles

Custom CSS for VSCode's Markdown preview, served via [jsDelivr](https://www.jsdelivr.com/).

## Setup

Add to `settings.json`:

```json
"markdown.styles": [
  "https://cdn.jsdelivr.net/gh/petchvm/markdown-styles@main/main.css"
]
```

> Raw GitHub URLs won't work in VSCode's preview; jsDelivr is whitelisted.

## What's in `main.css`

- **Inter** with OpenType features (`cv02`, `cv03`, `cv04`, `cv11`)
- Centered layout capped at 800px
- Tighter heading letter-spacing
- `text-wrap: pretty` for body, `balance` for headings

## Updating

1. Edit and commit the file.
2. Purge the jsDelivr cache: `https://purge.jsdelivr.net/gh/petchvm/markdown-styles@main/main.css`
3. Reload the Markdown preview in VSCode.
