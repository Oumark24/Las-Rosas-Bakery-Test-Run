# Rosa's Bakery

A single-page website for **Rosa's Bakery**, a 24-hour Mexican bakery at 5824 4th Ave in Sunset Park, Brooklyn. One static `index.html`, no framework, no build step, no backend, deployed to GitHub Pages.

**Live site:** https://oumark24.github.io/Las-Rosas-Bakery-Test-Run/

## What it does

- **Menu with an order cart** — conchas, churros, tres leches, tamales and custom cakes can be added to an order with per-item quantities and a live total. The cart persists in `localStorage` under `rosasCart`, so a customer can keep browsing without losing their order.
- **Phone-ready checkout** — checkout builds a plain-text order summary ending in *"Call (718) 492-1470 to place this order."* The bakery takes orders over the phone, so the site hands off cleanly instead of faking a payment step.
- **Category filtering** — the menu switches between categories in place, which keeps a long bakery menu usable on a phone screen.
- **Search and social metadata** — `Bakery` JSON-LD including the address, phone, and `Mo-Su 00:00-23:59` opening hours (the bakery really is 24 hours), plus Open Graph and Twitter card tags for link previews.

## Why it's built this way

The whole site is one file because the content is one page. There's no build step to break, nothing to install, and the client can edit copy or prices directly. Hosting on GitHub Pages costs nothing and updates on push.

Marking the hours as `00:00-23:59` in structured data is what makes Google surface the bakery as open around the clock — a small detail that matters more to this business than any visual feature.

## Running it

```bash
git clone https://github.com/Oumark24/Las-Rosas-Bakery-Test-Run.git
cd Las-Rosas-Bakery-Test-Run
open index.html
```

## Deployment

`.github/workflows/static.yml` publishes the repository root to GitHub Pages on every push to `main`.

## Files

| Path | Purpose |
| --- | --- |
| `index.html` | Entire site — markup, CSS, menu data, cart and checkout logic |
| `favicon-192x192.png` | Favicon |
| `.github/workflows/static.yml` | GitHub Pages deployment |
