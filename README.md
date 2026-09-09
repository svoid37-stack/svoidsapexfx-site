# svoidsapexfx.com

Marketing and storefront site for svoidsapexfx — Apex Legends overlays and
stream FX.

Static single page, no build step. `index.html` is the whole site; the only
external dependency is Google Fonts (Teko and Saira Condensed), which the
overlay products use too.

## Publishing

Served by GitHub Pages from `main`, at the apex domain in `CNAME`.

DNS records needed at the registrar:

| Type | Name | Value |
|---|---|---|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `svoid37-stack.github.io.` |

Turn on **Enforce HTTPS** in Settings → Pages once the certificate is issued.

## Before this goes live

- [ ] Set the real price (`$XX` placeholder in the buy panel)
- [ ] Wire the Get the overlay button to the store checkout (`#buyBtn`)
- [ ] Confirm the contact address exists on the Workspace account

## Product source

The overlay itself lives in the private `Apex-Overlay` repo. It is deliberately
not in this repo — this one is public.
