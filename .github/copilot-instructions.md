<!--
Guidance for AI coding agents working on this repository.
Keep instructions concise and only change files that are clearly needed.
-->

# Copilot / AI Agent Instructions

Purpose
- This repository is a tiny static site: the entire app is a single file at `index.html`.

Big picture
- Single-page static HTML (no JS frameworks, no build or test tooling).
- Primary surface: [index.html](index.html) — edit this file for UI/content changes.

What to do first
- Open and inspect `index.html` to understand structure and inline styles.
- If you need to run the site locally, serve the folder (example):

```bash
python3 -m http.server 8000
# then open http://localhost:8000/index.html
```

Project-specific conventions
- Keep changes minimal and self-contained in `index.html` unless user requests otherwise.
- Do not introduce frameworks, package.json, or build tooling without explicit instruction.

Integration points & external deps
- There are currently no external services, APIs, or package dependencies.

Commit / editing guidance
- When modifying `index.html`, prefer small, reversible patches.
- If adding files (assets/css/js), place them at the repo root or a new `assets/` folder and update `index.html` references.

When merging into an existing `.github/copilot-instructions.md`
- Preserve existing high-value content. Append or replace only clearly outdated lines and keep intent intact.

Examples from this repo
- To change text content or layout, update [index.html](index.html) directly.
- To preview changes, run `python3 -m http.server` and load `index.html` in a browser.

When to ask the user
- Ask before adding a build tool, dependency manager, or major project restructure.
- Ask before removing or renaming `index.html`.

If tests or CI are needed
- There are no tests or CI configured. Propose a minimal plan and ask the user before adding workflows.

End
- Ask the user for clarification if any requested change is larger than a small edit to `index.html`.
