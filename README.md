# Noted website

The landing page for Noted, the AI voice planner for iPhone. Plain static HTML and CSS with no build step, deployed on Vercel.

| Page | File |
|---|---|
| `/` | `index.html` (English) |
| `/ar` | `ar.html` (Arabic, right-to-left) |
| `/privacy` | `privacy.html` |
| `/support` | `support.html` |
| 404 | `404.html` |

`privacy.html`, `support.html` and `404.html` are generated from the app's privacy text, so the website and the in-app privacy screen always match. To regenerate them after changing the text, run `python3 worker/scripts/build_pages.py` in the app repo (`../noted`).

To preview locally, run `npx vercel dev` (or any static server; the clean URLs like `/ar` need Vercel's `cleanUrls`).

Fonts are subsets of Inter, Inter Tight and DM Mono, released under the SIL Open Font License (`fonts/OFL.txt`).
