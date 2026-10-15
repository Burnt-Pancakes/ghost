# Aether Arcanum theme

This fork of Mapache was reworked into a dark, terminal-style theme (sidebar nav, hero, latest-post strip, feature cards, news feed).

- `default.hbs`: new shell (sidebar, top bar, footer). No longer loads Mapache `main.css` / `main.js`.
- `index.hbs`, `post.hbs`, `page.hbs`, `tag.hbs`, `author.hbs`, `error-404.hbs`: rewritten.
- `partials/ae-sidebar.hbs`, `partials/ae-card.hbs`: new partials.
- `assets/styles/aether.css`: all styling, plain CSS (no gulp/tailwind build needed).
- Mobile: sidebar collapses into a sticky top bar with a CSS-only menu; grids drop to 2 then 1 column.

Edit the hero headline, feature cards and terminal box text directly in `index.hbs` / `partials/ae-sidebar.hbs`.
Navigation comes from Ghost Admin > Settings > Navigation (primary = sidebar list, secondary = social links).

Install: zip the repo root (without .git) and upload in Ghost Admin > Settings > Design > Change theme.
Legacy Mapache templates (`godo-*`, `custom-*`, `amp.hbs`) and the old partials are left in place but unused by the new layout.
