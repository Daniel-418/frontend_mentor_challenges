# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a [Frontend Mentor](https://www.frontendmentor.io) challenge — a static blog preview card built with plain HTML and CSS. No build tools, frameworks, or package managers are used.

## Development

Open `index.html` directly in a browser to preview the component. There are no build steps, servers, or test suites.

## Architecture

- `index.html` — single page with the card component markup
- `style.css` — all styles; uses CSS custom properties defined in `:root`
- `assets/fonts/` — local Figtree variable font (wght axis, weights 500 and 800)
- `assets/images/` — card illustration, avatar, and favicon
- `design/` — reference JPGs (mobile, desktop, active states) to match pixel-for-pixel

## Design Tokens (from `style-guide.md`)

| Token | Value |
|---|---|
| Primary yellow | `hsl(47, 88%, 63%)` |
| White | `hsl(0, 0%, 100%)` |
| Gray 500 | `hsl(0, 0%, 42%)` |
| Gray 950 / black | `hsl(0, 0%, 7%)` |
| Font family | Figtree (local TTF) |
| Font weights | 500 (medium), 800 (extra bold) |
| Base font size | 16px |
| Breakpoints | mobile 375px, desktop 1440px |

## Key Implementation Details

- Layout: `body` uses a 3×3 CSS Grid to center the card both horizontally and vertically.
- Card shadow: `8px 8px 0px 0px black` hard offset (no blur), matching the design's flat shadow style.
- Hover interaction: `.card-title` transitions `color` to the primary yellow on hover.
- The Figtree font is self-hosted via `@font-face` pointing to the local variable font file.
