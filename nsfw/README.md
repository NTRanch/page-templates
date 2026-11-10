# TEMPLATE — NSFW Game Page

Canonical source: [`description.html`](description.html) in this folder.
This is the spec as designed on 2026-11-09. (The itch-side draft could
not be created that day — the account's project cap refused a fifth
project — which is one reason the templates live here now.)

## Fields

- **Title:** the game's name
- **Tagline pattern:** `[A/An] [genre] [form] — 18+`
- **Pricing:** $0 or donate
- **Classification:** Games / Downloadable / In development (until the build locks)
- **Genre:** pick per game
- **Tags:** up to 10, per game
- **Community:** Comments
- **Sensitive content:** **checked** — Metadata → Classification →
  "Has sensitive content" (the adult-content flag; "Show content
  warning" is also offered there)

## The standing adults-only block

The description opens with it, always, before the pitch:

- Heading: "18+ — Adults Only"
- The notice paragraph (adult content, 18+ only, per-game additions)
- "Content notes" with the game's actual content notes filled in
- The line: "All characters depicted are adults."

## Theme (set in the public page's Edit theme panel)

| Field | Value |
| --- | --- |
| Background | `#0f0f0f` |
| Background 2 | `#1a1a1a` |
| Text | `#f5f5f5` |
| Link | `#c1121f` |
| Headers | `#e5484d` |
| Buttons | `#a4161a` |
| Font | Lato |
| Size | Large |
| Screenshots layout | Auto |
| Banner / background image | none in the template; per game |

## Notes

- The links row (GitHub · License · Patreon) is a centered paragraph of
  plain links — itch descriptions cannot carry styled buttons or
  embedded badge images (see the repo README's mechanics box).
- The "Built with" badge URLs are links on itch and real badges on
  GitHub. Swap label, version, color, and logo slug per game.
