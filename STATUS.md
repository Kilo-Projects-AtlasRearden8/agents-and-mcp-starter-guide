# STATUS

## What was built

A beginner manual on AI agents and the Model Context Protocol (MCP), delivered in two formats:

- **docs/** — Markdown source (6 files): welcome, what AI agents do, how MCP servers work, running your first stdio server, safety rules for file access, master checklist.
- **site/** — Static HTML website (7 HTML files + 1 CSS file) mirroring the docs, fully offline usable.
- **README.md** — project overview, contents table, credits Asdale Dynamics, LLC.
- **LICENSE** — MIT License with copyright line exactly `Copyright (c) 2026 Asdale Dynamics, LLC`.
- **STATUS.md** — this file.

## How to run it

- Markdown: open any file in `docs/` with a text editor or view on GitHub.
- HTML site: open `site/index.html` in any browser. No build step, no server, no internet required. All pages link to one another via `site/style.css`.

## Verification results

- All 6 HTML pages and `index.html` parsed without error.
- Every internal link across the site resolves to an existing file (0 broken links).
- Every page includes `<title>` and links to `style.css`.
- `LICENSE` contains the exact copyright line `Copyright (c) 2026 Asdale Dynamics, LLC`.
- `README.md` credits Asdale Dynamics, LLC.
- Git initialized and committed as a single root commit (plain message, no co-author trailers). Nothing pushed; no remote created.

## Known gaps

- No automated test suite or CI configured (none requested; no `.github/workflows` added).
- The stdio server commands reference third-party tools (Node.js/npx, @modelcontextprotocol/server-filesystem, an MCP-compatible AI client) that must be installed separately; they are not bundled or tested offline in this repo.
- No browser-based accessibility audit performed beyond semantic markup and alt-free structural pages.
