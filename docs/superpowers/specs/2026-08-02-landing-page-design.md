# Landing Page Design — code-kitchen (ck.uy)

## Summary

Single-file HTML landing page for Code Kitchen, deployed via GitHub Pages and served at ck.uy.

## Visual Design

- **Theme:** Dark hacker-kitchen — terminal aesthetic with kitchen metaphors
- **Background:** `#0a0a0a` with a faint CRT scanline overlay (CSS repeating-gradient, ~2px pitch)
- **Font:** JetBrains Mono (Google Fonts CDN)
- **Accent color:** `#00ff88` (terminal green)

## Layout

Full-viewport, vertically and horizontally centered column with three elements:

1. **Heading** — "Code Kitchen", large (~10–12vw), white with green `text-shadow` glow
2. **Tagline** — `> We are cooking something awesome.` with typewriter animation + blinking block cursor
3. **Footer** — `© 2026 Code Kitchen SAS — All rights reserved.`, small, dimmed, fixed to bottom

## Animations

| Element | Animation | Timing |
|---------|-----------|--------|
| Heading | Fade in on load | 0.6s ease |
| Heading (hover) | CSS glitch (color-channel split flicker) | 300ms |
| Tagline | Typewriter, character by character | ~60ms/char |
| Cursor | Blink after typewriter completes | 600ms interval |

## Files

- `index.html` — single file, all CSS and JS inline
- `CNAME` — contains `ck.uy` for GitHub Pages custom domain

## Deployment

- GitHub Pages from `main` branch root
- Custom domain set via `CNAME` file + DNS `A` records pointing to GitHub Pages IPs
