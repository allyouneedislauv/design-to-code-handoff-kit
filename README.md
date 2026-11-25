# Design-to-Code Handoff Kit

Design tokens for a Figma component kit, mirrored as code-ready files. Built to show how a Figma Variables architecture can map directly to what a developer would actually use.

## What's inside

- `tokens.json`: tokens in the W3C Design Tokens format (`$value` / `$type`), with semantic tokens aliasing primitives
- `tokens.css`: the same tokens as CSS custom properties

## Token architecture

Tokens are organized in two layers:

- **Primitives**: raw values (e.g. `--blue-600: #4A6FD1`)
- **Semantic**: usage-based names that alias primitives (e.g. `--color-primary: var(--blue-600)`)

Components only reference semantic tokens. Changing a brand color means editing one primitive, and everything that depends on it updates, the same DRY principle applied to design.

## Covers

Color, spacing, border radius, and one shadow effect. Typography isn't tokenized in this version.

## Accessibility note

The original light blue (`#7C9FE8`) failed WCAG AA with white text (~2.6:1). `#4A6FD1` (~4.7:1) is the functional primary for anything carrying text; the lighter blue is kept for backgrounds and hover fills.

## Notes

The files are maintained manually to match the Figma Variables. There is no automated sync or build step.

## Links

- Case study: https://www.allyouneedislauv.com/
- Figma file: _add link once published_

Built by Laura Hundzinski da Rocha (Lau), Product Designer.
