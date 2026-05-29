# Eva Lyneborg — Logo System

## Working with the project owner

The owner (Frits) is a **designer and architect, not a technician**.

- **Do technical work yourself.** Do not ask Frits to run CLI commands, install
  tools, configure auth, edit files, or perform other technical steps that you
  are capable of doing. Just do them.
- Only involve Frits in **design and architecture decisions** — look & feel,
  naming, behavior, product direction, tradeoffs that change the outcome.
- If a technical action genuinely requires a human (e.g. an interactive
  login you truly cannot complete, or a permission only they can grant),
  explain it in plain, non-technical language and keep their effort minimal.

## Project overview

A browser-based **Logo Studio** for producing alternative versions of the
Eva Lyneborg logo. Pure static front-end (HTML/JS/SVG) — runs entirely in the
browser, no backend. Intended to be hosted online (GitHub Pages) as an
always-available internal tool.

### Key files
- `index.html` — the Logo Studio app
- `LOGO.svg` — base logo (note: filename is uppercase; matters on Linux hosts)

### Current features
- Fill color, background color (pickers + hex)
- Height regulator — moves the top bar of the frame (−125 → +109), view
  auto-expands so nothing clips
- Swap colors / Reset

### Roadmap
- Text-entry workflow for named logo variants
- Independent coloring of frame vs. face
- Client-side SVG export

### Running locally
Served over HTTP (the page `fetch`es the SVG, so `file://` won't work):
`python -m http.server 8777` → http://localhost:8777/index.html
