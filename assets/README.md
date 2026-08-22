# Las Rosas Bakery — Asset Handoff Guide

This static site intentionally uses a lightweight CSS editorial treatment until approved business photography is available. It does not use stock photography, generated food images, remote image placeholders, or encoded assets.

## Existing asset

| File | Purpose | Replace? |
|---|---|---|
| `../favicon-192x192.png` | Current compact brand mark used in the header and browser icon | Replace only when an approved, clean logo export is supplied. Keep the filename or update its HTML reference in `index.html`. |

## Recommended future local assets

Place approved files in the folders below. Keep filenames descriptive and update the clearly marked `<!-- ASSET: ... -->` comments in `index.html`.

| Suggested file | Use | Recommended treatment |
|---|---|---|
| `hero/las-rosas-storefront.webp` | Optional hero/storefront photograph | WebP, landscape crop, approximately 1600px wide, compressed before upload. Add as a CSS background only after approval. |
| `gallery/pan-dulce-case.webp` | Optional counter/gallery image | WebP, responsive dimensions, lazy-load below the fold. |
| `gallery/cakes-counter.webp` | Optional custom-cake image | WebP, responsive dimensions, lazy-load below the fold. |
| `logo/las-rosas-logo.png` | Clean logo for header/social sharing | Transparent PNG or SVG, cropped with no screenshot background. |
| `social/las-rosas-social-preview.jpg` | Optional sharing image | JPG or PNG, 1200 × 630px, a real approved storefront or bakery image. |

Do not upload base64-encoded assets. Do not use unapproved food photography, stock photography, or AI-generated food imagery as a substitute for real business assets.

## Premium visual treatment

| File | Purpose | Public-facing constraint |
|---|---|---|
| `visuals/pastry-paper-material.webp` | Earlier local abstract paper-material treatment retained as a supporting visual | Do not represent it as the storefront, logo, staff, inventory, menu, or food photography. It remains a non-documentary visual treatment only. |
| `visuals/hero-paper-sculpture.jpg` | Primary motion-hero material, generated as an abstract folded-paper and geometric-material study | It is not a photo of Las Rosas, its food, staff, storefront, inventory, menu, packaging, or logo. Use only as a non-documentary visual layer in the homepage hero; do not reuse it as factual business photography. |

The cinematic hero keeps both a high-contrast readability overlay and CSS 3D foreground planes in `index.html`; its page copy and customer actions remain independent of the visual. Replace the material only with owner-approved documentary imagery or an equally non-documentary local treatment.
