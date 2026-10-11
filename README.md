# svgproxy-jsdelivr

Remake of [Mo9nikeypurple/svgproxy](https://github.com/Mo9nikeypurple/svgproxy) that loads **all assets via jsDelivr**.

## What changed

- `index.html` — CDN loader config points to `https://cdn.jsdelivr.net/gh/Mo9nikeypurple/svgproxy@main/` (+ Fastly/Gcore mirrors)
- `index.svg` — every script, stylesheet, favicon, and service-worker URL is an absolute jsDelivr link
- Service worker registration uses the original repo’s worker hosted on jsDelivr

## Usage

**HTML entry**
```
https://cdn.jsdelivr.net/gh/mathissofun137/svgproxy-jsdelivr@main/index.html
```

**SVG entry** (common for filter bypass)
```
https://cdn.jsdelivr.net/gh/mathissofun137/svgproxy-jsdelivr@main/index.svg
```

Or open the raw files directly from this repo.

Assets (JS bundles, CSS, fonts, images) continue to be served from the upstream `Mo9nikeypurple/svgproxy` repository via jsDelivr, so this repo stays tiny.
