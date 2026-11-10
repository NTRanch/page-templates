# Page Templates — Nice Thoughts Ranch

The studio's itch.io page templates, kept here on GitHub instead of as
itch draft projects: versioned, clonable, and not hostage to itch's
project cap or editor limits.

Two lanes, kept separate:

- [`sfw/`](sfw/) — the SFW game page template (light theme, no content block)
- [`nsfw/`](nsfw/) — the NSFW game page template (dark theme, standing 18+ block, adult-content flag)

Each lane folder holds:

- `description.html` — the canonical page description skeleton. Every
  `[BRACKETED]` line is a per-game fill-in.
- `README.md` — the lane's tagline pattern, pricing, classification,
  and exact theme values.

## How a template becomes a page

1. Create the itch project (draft) when the account's project limit allows.
2. Rebuild the description in itch's editor from `description.html`.
   Do not paste the HTML into the editor's source view — see the
   mechanics box below. The structure is headings, paragraphs, lists,
   one table, and a centered link row; all of it is toolbar work.
3. Set the theme values from the lane README (the theme editor lives in
   the public page's **Edit theme** panel, not on the edit page).
4. Set classification, genre, and up to 10 tags; confirm pricing
   ($0 or donate) and keep the page Draft until the launch checklist passes.
5. Upload the assets (specs below) and the game files — butler for game
   files, the editor for images.
6. Replace the Status line in the same step as any upload. Public copy
   describes the build that ships, in plain language — no internal
   codenames, no mechanic names a stranger can't parse.

## itch editor mechanics (probed 2026-11-09, three rounds)

- **Source-view HTML never reaches the server.** The editor's Save
  submits only its visual (toolbar) model. Anything pasted as raw HTML —
  inline styles, styled buttons, `<hr>`, pasted iframes, external
  `<img>` tags — is silently dropped.
- **What persists:** Heading 2, bullet lists, tables (plain cells),
  centered paragraphs, links (with open-in-new-tab), and YouTube/Vimeo
  embeds made with the editor's Video button or the edit page's
  "Gameplay video or trailer" field.
- **Images are upload-only.** The Add image control takes gif / jpeg /
  jpg / mp4 / png up to 3 MB. Externally hosted images — including
  shields.io badges — cannot be embedded in a description at all.
  Badges therefore ship in the templates as links; on GitHub (repo
  READMEs, release notes) the same badge URLs render as real badges.
- **No custom CSS exists** in the game-page theme editor. Visual appeal
  comes from theme colors, fonts, layout, and the description's own
  structure — that's why the templates specify exact theme values.
- **Buttons on itch** are either the templates' centered link row or
  uploaded button images. There is no third option.

## Asset specs

| Asset | Spec |
| --- | --- |
| Cover image | 630×500 recommended (315×250 minimum) |
| Screenshots | 3–5, of the actual build |
| Gameplay GIF | 3–6 second loop, ≤ 3 MB via Add image, or as a screenshot |
| Trailer | YouTube or Vimeo link in the "Gameplay video or trailer" field |
| Background / banner | Theme panel uploads; use a wide image |
| Game files | Butler channels: linux / windows / android / web; version scheme `0.1.0-<slice-name>` |

## Launch checklist (per game)

- [ ] Every `[BRACKETED]` placeholder replaced
- [ ] Tagline follows the lane pattern (genre + form, plain language)
- [ ] Links row points at this game's repo, its LICENSE, and the studio Patreon
- [ ] Badge links carry this game's real stack and versions
- [ ] Genre picked, tags set (up to 10)
- [ ] NSFW lane: "Has sensitive content" checked, content notes filled in
- [ ] Cover, screenshots, GIF, trailer in place
- [ ] Build uploaded via butler and launch-verified
- [ ] Status line matches the shipped build
- [ ] Pricing $0 or donate confirmed; visibility switched only now
