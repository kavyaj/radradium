# Radradium (radradium.com)

The company site for Radradium, a small web studio registered in Singapore (UEN 202124283W). One page that shows everything the company makes, as a periodic table: Radradium is element 88 and every project takes the next number in launch order.

## Stack

- Plain static HTML and CSS. No framework, no build step, no npm.
- Hosted on GitHub Pages with the custom domain in `CNAME`. `.nojekyll` stays.
- Fonts are self-hosted, subset woff2 files in `assets/fonts/`. Never add Google Fonts or other third-party requests.
- No analytics or trackers unless Kavya asks for them.

## Files

- `index.html`: the homepage. Its `<head>` holds all SEO tags and the JSON-LD.
- `404.html`: GitHub Pages serves it for missing paths.
- `design/`: the brand source of truth. `brand-book.md` has the rules, `tokens.json` and `tokens.css` have the values. Read `brand-book.md` before changing anything visual.
- `assets/img/`: logo SVGs (never redraw or recolour them) and `radradium-mark.png` (the JSON-LD logo).
- `og-image.png` (1200×630), favicons, `site.webmanifest`, `robots.txt`, `sitemap.xml`.

## Brand rules that bite

- Light site only. The only dark surface is `dial` (#0f1a14), and only inside product cards and tiles.
- Glow, not gloss: no sheen, glare, highlight rims or gradient fills. The one light effect is the radium text-shadow on symbols.
- Products lead, then the one service (Red Thread Careers), then side projects in the small "By the way" strip. Never promote a side project above it.
- Tile colour follows category: products `dial`, service `radium`, side projects white.
- Every outbound link has `target="_blank" rel="noopener noreferrer"` and ends with `↗`. In-page anchors don't.
- Copy voice: short sentences, contractions, wry and specific. Never em dashes. Never "landscape", "leverage", "game-changer", "unlock", "delve", "quietly", or "This isn't X, this is Y".

## Adding a new project

1. Give it the next free number (96 is next) and a two-letter symbol.
2. Add it to the hero periodic grid, its section (Products, Service or By the way), the JSON-LD `brand` list, the element table in `design/brand-book.md`, and regenerate `og-image.png` if the grid changed.
3. Update `<lastmod>` in `sitemap.xml`.

## Checks before every push

- The page works at 390px wide with no horizontal scroll.
- One `<h1>`. Every image has `alt` (decorative ones `alt=""`).
- Lighthouse (mobile) Performance, Accessibility, Best Practices and SEO all 95 or higher.
- The JSON-LD validates at https://validator.schema.org.
