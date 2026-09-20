# Rhubarb — Three Hero Skeletons

Build THREE files, each a hero section only. Nothing scrollable beneath — one viewport each, then stop. These are direction tests, not pages.

## Shared rules (all three)

- Tailwind via CDN, single self-contained file each, no build step.
- Colors: cream `#F4EDDC`, red `#AE3220`, ink `#191713`. No other colors.
- Type: Poppins 900 for display and the wordmark, Figtree for body, JetBrains Mono for small labels (uppercase, letterspaced).
- Wordmark: the word `rhubarb`, lowercase, Poppins 900, ink (or cream on dark grounds). Text, not an image. Never paired with an icon.
- Photo: `assets/rhubarb-hero.avif`, `<picture>` with `assets/rhubarb-hero.jpg` fallback. It's square — `object-fit: cover`, and keep `object-position` on its own line so it's easy to tune.
- Headline everywhere: `Your future is right behind you.`
- Subhead where one fits: `Rhubarb designs and builds backyard homes tailored to your lot and your life.`
- CTA: one red button, `GET GROWING`, JetBrains Mono, uppercase.
- Nav links where a nav wants them: `BUILDINGS · PROCESS · PRICING · ABOUT` (dead links).
- Responsive to 375px. No animation anywhere yet.

## hero-1-fullbleed.html — photo as atmosphere

- Photo full-bleed, 100vh.
- Floating pill nav, centered, ~24px from the top, detached from all edges: wordmark left, the four links center, GET GROWING right. Frosted — `backdrop-filter: blur` with a translucent cream tint, subtle border. This nav is the signature of this version; spend the effort here.
- Headline + subhead + CTA anchored in the LOWER THIRD of the image, left-aligned, over the flower bed (the darkest zone). Cream type. A subtle bottom-up gradient scrim (transparent → ink at low opacity) behind the text zone only — never a full-image darkening.

## hero-2-split.html — photo as evidence

- Ground: cream page (this version's ground is cream, not white).
- Top bar, not floating: wordmark left, links + GET GROWING right, generous padding.
- Headline huge, left-aligned, ink on cream, max 3 lines, occupying the upper zone. This version lives or dies on type scale — err larger.
- Below the headline, a metadata row split left/right in mono: left `BACKYARD HOMES · DENVER`, right `FROM $400K · DESIGN THROUGH MOVE-IN`. Thin ink rules above it.
- Photo full-width beneath, top-cropped by the fold so it clearly continues below — it should feel cut off by the viewport, not contained by it.

## hero-3-field.html — image as object

- Ground: solid cream, 100vh, edge to edge.
- Wordmark and nav words pushed to the extreme corners/edges of the viewport, mono, small: `rhubarb` top-left, links spread across the top edge with large gaps, GET GROWING top-right as red text (no button fill in this version).
- The photo small — roughly 420px square — dead center, no border, no caption.
- Headline set small and quiet, bottom-left. Mono label bottom-right: `SCROLL & DISCOVER`.
- The emptiness is the design. Resist filling it.

## Also build

`index.html` — three links, plain, nothing else.

Build all four files, then stop. No variants, no extra ideas.
