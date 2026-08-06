# Critical Collective — static site

A plain static build: no bundler, no build step. Open `index.html` or serve the folder.

## Layout
- `index.html` and the other page files — one per screen
- `CC Header.dc.html`, `CC Footer.dc.html` — shared header/footer, loaded at runtime
- `support.js` — runtime that renders the pages (must sit beside the pages)
- `image-slot.js` — image placeholder component
- `_ds/classical-.../` — design-system stylesheet + bundle (tokens, components)
- `assets/` — logos and photographs
- `newsletter-august-2026.html` — standalone HTML email

## Pages
| File | Screen |
| --- | --- |
| index.html | Home |
| contents.html | Contents / site index |
| modern-contemporary-art.html | Modern & Contemporary Art |
| art-history-museums.html | Art History & Museums |
| cinema-photography.html | Cinema & Photography |
| cinema-ott.html | Cinema & OTT department |
| lens-based-practices.html | Lens-Based Practices department |
| art-design-architecture.html | Art, Design & Architecture |
| culture.html | Culture |
| article.html | Article |
| art-history.html | Art History — four standing dossiers |
| artists.html / artist.html | Artists index / artist page |
| authors.html / author.html | Authors index / author page |
| newsletters.html | Newsletters |
| reference.html | Reference & Archives |
| search.html | Search (accepts `?q=`, `#field=`, `#tag=`) |
| signin.html | Sign in / subscribe |
| about.html, contact.html, privacy.html, donate.html | Institutional pages |

## Deploying
Any static host. For GitHub Pages, push the folder contents to the branch Pages serves; `.nojekyll` is already present so `_ds/` is published.
