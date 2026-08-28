# CLAUDE.md

day14 — static landing page for the "MVP in 2 weeks" agency (£9,950 fixed). GitHub Pages serves `index.html`
from `main`; `CNAME` binds the custom domain.

## Hard rules

- **Branch → PR, never commit to `main`** — a merge to `main` IS the deploy. No AI attribution in commits/PRs.
- **Do not touch `CNAME`** unless the owner explicitly says the domain changed (domain state has a history of
  registrar trouble — the owner tracks it).
- Single-file site by design: keep it one `index.html`, inline CSS/JS, no build step, no frameworks.
- Copy states the real offer only — price, scope, and timeline come from the owner; never invent testimonials,
  logos, or client counts.

## Checks

Open `index.html` locally in a browser; verify mobile layout (≤390px), all anchors, and that the page still
loads with JS disabled. No tooling exists in this repo — that is deliberate.
