# CLAUDE.md

## Project

Static pitch deck for SANA (sanacompany.io). Single `index.html` with inline CSS/JS. No framework, no build step.

## Key Files

- `index.html` — entire presentation: markup, styles (~1800 lines of CSS), and JS
- `translations.json` — all user-facing text in EN and KR
- `assets/` — images grouped by section (ai, brand, clients, crypto, games, iot, robotics)

## Architecture

- Slide-based layout using CSS scroll-snap on `.slide-container`
- Each slide is a `<section class="slide">` with a `data-slide` attribute
- Navigation handled in JS: keyboard (arrows/space), touch (swipe), and nav dots
- Language toggle swaps text by reading keys from `translations.json`
- Theme uses CSS custom properties (--gold, --turquoise, --blue, --magenta on dark bg)

## Development

```bash
pnpm install && pnpm dev   # serves on localhost:3000
```

## Deployment

GitHub Pages from `main` branch, root `/`. Live at sanacompany.io/sana-pitchdeck/.

## Style Notes

- Fonts: Bebas Neue (display), Cabinet Grotesk (headings), General Sans (body)
- All sizing uses `clamp()` for responsive typography
- Dark theme: `--bg-primary: #08080c`
- Brand colors: gold (#F5C542), turquoise (#3DD9B6), blue (#0066ff), magenta (#FF0080)
