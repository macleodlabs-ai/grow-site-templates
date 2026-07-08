# grow-site-templates

Theme and template presets for [Grow](https://grow.macleodlabs.com)'s generated websites.

**Data only, never code.** Each theme is a JSON file: a complete light + dark palette pair
(WCAG ≥4.5:1 body-text contrast, computed), a display-font stack (system stacks only —
generated pages load no external fonts), radius/spacing hints, and section-layout notes.
The Grow app pulls `themes/index.json` at publish time (cached, validated, with built-in
fallbacks) — so new themes ship here without an app deploy.

## Adding a theme
1. Copy an existing `themes/<name>.json`, change the tokens.
2. Verify contrast: every `ink`/`inkMuted` must hit ≥4.5:1 on `bg` AND `surface` in BOTH modes.
3. Add the name to `themes/index.json`.

## Schema
See `themes/evidence.json` — the reference theme (Grow's own evidence-paper look).
