# Eva Lyneborg — Logo System

A small browser-based **Logo Studio** for producing alternative versions of the
Eva Lyneborg logo for different uses.

## Current features

`index.html` loads the base logo (`LOGO.svg`) live and lets you adjust:

- **Fill (artwork)** — color of the logo, via color picker or hex field
- **Background** — background color, via color picker or hex field
- **Height regulator** — moves the top bar of the frame up or down
  (−125 → +109); the view expands automatically so the frame is never clipped
- **Swap colors** / **Reset**

## Running locally

The page inlines the SVG via `fetch`, so it must be served over HTTP
(not opened as a `file://` URL):

```bash
python -m http.server 8777
# then open http://localhost:8777/index.html
```

## Roadmap

- Text-entry workflow for generating named logo variants
- Independent coloring of the frame vs. the face
- Export (PNG / SVG) with a view that grows to fit any adjustment
