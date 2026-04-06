# Lazaderm landing pages

Static HTML marketing landers for **Lazaderm**—location-focused campaigns and procedure/service campaigns. Each page is self-contained (inline CSS, no build step).

## Contents

| Type | Hub | Notes |
|------|-----|--------|
| **Index** | [`index.html`](index.html) | Internal directory of all landers (`noindex`). |
| **Location landings** | — | e.g. `chandler-landing.html`, `fargo-nd-landing.html`, `sioux-falls-sd-landing.html`, `sioux-city-ia-landing.html`, `watertown-sd-landing.html` |
| **Procedure landings** | — | e.g. `coolsculpting-elite-landing.html`, `dermal-fillers-landing.html` |
| **Template** | — | [`procedure-landing-template.html`](procedure-landing-template.html) — duplicate to start a new procedure page |

Markdown briefs (`Lazaderm_L_*_BH.md`) sit alongside the HTML and hold copy/source of truth for new or updated pages.

## Preview locally

There is no package manager or compile step. Open any `.html` file in a browser, or serve the folder:

```bash
cd LazadermLanders
python3 -m http.server 8080
```

Then visit `http://localhost:8080/` (start from `index.html` if you want the directory).

## Adding a new procedure landing

1. Copy `procedure-landing-template.html` to a new file (e.g. `my-service-landing.html`).
2. Replace placeholders, meta title/description, hero, sections, FAQs, and CTAs to match the markdown brief.
3. Add a card linking to the new file in `index.html` under **Procedure landings**.

## Deployment

Upload the HTML assets to your host or CDN as usual. Ensure form embeds and external links are updated for production.

## License

Proprietary — Lazaderm. All rights reserved unless otherwise agreed.
