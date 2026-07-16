# AGENTS.md

## What this repo is

Design + project workspace for the Susan Allen, LMFT engagement (WFC client). **Not a software project** — no build, test, lint, or typecheck commands exist. Contents are static HTML mockups, markdown docs, and a YAML token file.

The Obsidian vault at `~/workspace/leads/wfc-susan-allen/` is the canonical source for engagement docs; `docs/` here is a read-mostly mirror. Mockups, design-system, and web-deliverable are the exception — they live in this repo as working source.

## Commands

There is nothing to run. To preview a mockup, open the HTML file directly in a browser (e.g. `open mockups/clove/index.html`). No dev server, no install step.

## Layout

- `mockups/<template>/index.html` — single-file self-contained HTML mockup of a Squarespace template, Susan's content + WFC tokens. Currently only `clove/` is built; `jenani/` and `clune/` are empty stubs.
- `design-system/` — WFC token layer + palette variants + PAD coordinates. **Token source of truth.**
- `docs/` — mirrored engagement docs (dossier, SOW, kick-off notes, 6-gate audits). Edit in the vault first, then re-mirror.
- `web-deliverable/` — pending Cloudflare Pages host for client review.
- `archive/` — superseded work.

## Conventions that differ from defaults

- **Token changes:** edit `design-system/` tokens first, then propagate the values into mockup `:root` blocks. Mockups embed tokens inline as CSS custom properties — keep them in sync.
- **Mockup rules:** single-file, no external deps, no build step. WFC tokens as CSS custom properties. `prefers-reduced-motion` media query required. WCAG 2.1 AA contrast. Fonts: Cormorant Garamond (display) + Atkinson Hyperlegible (body) via Google Fonts `<link>`.
- **Screenshots:** saved alongside the mockup as `screenshot-N-section.png` (e.g. `screenshot-1-hero.png`).
- **No pure black** (`#000`) — use WFC near-black (`#2C2825` for warm palettes, `#1F2A30` for cool).
- **Commits:** short imperative subject, body explains why. Co-authored-by trailer if Frank + Mavis both worked the change.
- **`.gitignore`** blocks large media (`.psd`, `.ai`, `.sketch`) and OS auto-screenshots, but explicitly allows `.gitkeep` and `README.md`.

## Client context (affects design decisions)

Susan's audience = reproductive + perinatal mental health = users who are anxious/overwhelmed. Mockup arousal targets run ~0.2 lower than WFC defaults. See `design-system/README.md` for PAD coordinates per page archetype. The 6-gate audit framework lives in `docs/audit-readme.md`.