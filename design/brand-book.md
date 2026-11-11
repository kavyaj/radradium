Radradium is a small web studio registered in Singapore. It makes web products, one service and a handful of free side projects. The brand is a periodic table: Radradium is element 88 (radium's real atomic number), and every project it launches becomes the next element.

## The idea in one paragraph

Radium glows. Watchmakers once painted it on dials so the numbers shone in the dark. Radradium borrows that: a light, paper-coloured site where the products sit on dark **dial** cards and their symbols glow **radium** green. The logo symbol is `Rr`, for Rad Radium. Numbers start at 88 and count up in launch order, so the homepage reads like a growing table of elements.

## Who the site is for

1. **The curious.** People who found one product (a BollyQuiz player, a StoryCV user) and clicked "made by Radradium" to see what else exists. They want the products, fast.
2. **The checkers.** Payment providers, ad platforms, partners, press. They want proof of a real company: registered name, UEN, a way to get in touch. They'll find it in the footer.

Everything on the page serves one of those two. If it serves neither, cut it.

## Page hierarchy

Products lead, the service follows. Use this order on every page that lists projects:

1. **Products** in `ElementCard` with `rr-card--product` (dial), three across.
2. **Service** in one `ElementCard` with `rr-card--service rr-card--wide` (radium).
3. **Company details** in `Footer`.

Side projects aren't featured on the homepage at all — no section, no hero tile. They still get an entry in the element table below, since a project keeps its number whether or not it's shown.

## The elements

| # | Symbol | Name | Category | Card |
| --- | --- | --- | --- | --- |
| 88 | Rr | Radradium | The company | `radium` tile, logo only |
| 89 | Rp | Resumey.Pro | Product | dial |
| 90 | Sc | StoryCV | Product | dial |
| 91 | Rt | Red Thread Careers | Service | radium |
| 92 | Mr | MRT Announcements | Side project | not on homepage |
| 93 | Ps | Poke & See | Side project | not on homepage |
| 94 | Bq | BollyQuiz | Side project | not on homepage |
| 95 | Ag | Again & Again | Product (new) | dial |

Rules: a project keeps its number forever, retired or not. A new project takes the next free number. Symbols are two letters from the name, first capitalised. Category decides the tile colour, never mood: products are `dial`, the service is `radium`. Side projects don't get a homepage tile or section.

## Voice

Write like Kavya talks: sharp, human, honest, occasionally wry.

- Short paragraphs, one to three sentences. Contractions always.
- Physical verbs for abstract ideas ("Talk through your work. Walk away with bullets.").
- Humour through specifics, not adjectives. "Singapore's train chimes, on tap" beats "a fun audio experience".
- Parenthetical asides are welcome (sparingly).
- Never: em dashes, "landscape", "leverage", "game-changer", "unlock", "delve", "quietly", or any "This isn't X, this is Y" line. No LinkedIn-speak.
- Product descriptions are one sentence, about 12 words, and say what the thing does for the person.
- The company is **Radradium** in running text and `radradium` (lowercase) only inside the wordmark.

## Colour

Light site, always. The only dark surface is `dial`, and only inside cards and tiles.

- Page: `paper`. Sunken bands (footer): `paper-2`. Raised paper: `paper-raised`.
- Text: `ink` for headings and body, `ink-2` for descriptions, `muted` for meta. On dial: `on-dial` and `on-dial-muted`.
- `radium` is a fill, never text on paper (it fails contrast). When radium needs to be text on paper, use `radium-deep`.
- `radium-glow` is light, not paint: halos around radium symbols only.
- Dividers: `line`. Borders a person must see: `line-strong`.
- Highlight a word in a headline with `.rr-mark`, a radium marker stroke under the lower half of the word. One per page.
- Focus ring: 2px solid `radium-deep`, 3px offset, on every interactive element.

## Type

- `display` (Unbounded, 600) for the hero, section titles, symbols and product names. Wide and geometric, like lettering on lab equipment. Tight tracking, never all caps.
- `sans` (Instrument Sans) for everything people read: `lead`, `body`, `body-s`, `button`.
- `mono` (JetBrains Mono) for readouts only: atomic numbers (`number`), tags and kickers (`label`, uppercase, 0.08em tracking), years and URLs.
- The hero uses `display-xl`; section titles `display-l`; card symbols `symbol` (or 96px on wide cards).

## Glow, not gloss

The brand glows; it never shines. Surfaces are flat colour.

- No sheen, glare, highlight rims or gradient fills on cards, tiles or buttons.
- The one light effect is the radium glow: a `text-shadow` in `radium-glow` and translucent `radium` around radium symbols on `dial`. On hover it brightens.
- Resting cards sit on `shadow-card`; on hover they rise 4px to `shadow-lift`.
- Buttons are keys with a solid ledge (`ledge-btn`, `ledge-radium`) that press flat on click.
- Respect `prefers-reduced-motion`: no lift or tilt.

## Links

Every link that leaves the page opens in a new tab: `target="_blank" rel="noopener noreferrer"`, and outbound link text ends with `↗`. In-page anchors (`#products`) stay in the same tab.

## Layout and shape

- Max content width 1120px, side margins `space-7`, sections separated by `space-8`.
- Cards: `radius-lg`, padding `space-5`, gap `space-5`. Small tiles: `radius-md`. Tags and URL pills: `radius-pill`.
- Grids are tile grids: square or two-wide cells, like a periodic table. Nothing is skewed or rotated except the small 1.5° tilt when a tile is hovered.

## Logo

Use the files in **Logos**: the radium mark for small spaces and favicons, the dial mark beside product cards and on socials, the wordmark in the header and on documents. Rules are in the Logo component. Never redraw it.

## Iconography

There are no icons. The element symbols are the icons. Use a text arrow (`↗`) for outbound links and a mono `·` as a separator. No emoji in the interface.

## Imagery

No stock photos, no screenshots inside cards. If a product page needs a picture, it lives on that product's own site.
