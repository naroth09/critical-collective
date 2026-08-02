# Critical Collective — site redesign

Static pages. Drop this folder into a repo, enable GitHub Pages, done — `index.html` is the front page and every path is relative.

`.nojekyll` is included on purpose: without it GitHub Pages ignores the `_ds/` folder (Jekyll skips directories starting with an underscore) and the site would load unstyled.

## Pages

| File | Page |
| --- | --- |
| `index.html` | Front page — hero carousel, four features, recent writing, index, ad banner, events ticker |
| `modern-contemporary-art.html` | Field 01 · Modern & Contemporary Art |
| `art-history-museums.html` | Field 02 · Art History & Museums |
| `cinema-photography.html` | Field 03 · Cinema & Photography |
| `art-design-architecture.html` | Field 04 · Art, Design & Architecture |
| `culture.html` | Field 05 · Culture |
| `artists.html` | Artist index, A–Z with live search |
| `newsletters.html` | Newsletter issues |
| `reference.html` | Reference & Archives |
| `search.html` | Faceted search — field, document type, era, tags |
| `signin.html` | Sign in, and the three plans (CC 1 $50 · CC 2 $75 · CC 3 $100) |
| `about.html` | About us |
| `contents.html` | Contents |
| `contact.html` | Contact |
| `privacy.html` | Privacy policy (draft) |

`CC Header.dc.html` and `CC Footer.dc.html` are the shared header and footer, imported by every page — change the nav or footer once, there. Keep those two filenames as they are; the import resolves by name.

## Supporting files

- `support.js` — component runtime, required by every page
- `assets/cc-logo.png` — logo, trimmed and knocked out to transparency (`cc-logo-source.png` is the original)
- `assets/hero-*.webp` — the three high-resolution hero photographs
- `_ds/classical-…/` — stylesheet and design tokens

## Brand values in use

Ground `#EFE8DD` · alternate band `#E5DBCC` · hairlines `#CDC3B3` · text `#000000` · editorial gold `#B8962E` for labels, rules and active states, with deep steps `#715A14` / `#56440F` on small text so it clears WCAG AA.

## Known gaps

- Article and artist links are placeholders — no article template yet.
- Listing images are hotlinked from criticalcollective.in and are only ~360px; they look soft at large sizes. Replace with high-resolution files when available.
- Carousel slide 3 (Satish Sharma) still uses one of those thumbnails.
- Forms (sign in, contact, subscribe) are not wired to a service.
- Privacy clauses pending.
