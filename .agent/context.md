```markdown
# Context: MrSpots1.github.io

## Project Summary
MrSpots1.github.io is a minimal GitHub Pages static website (https://mrspots1.github.io). It currently renders only the README.md as the homepage. Designed as a personal landing page; expand by adding static assets or Jekyll for dynamic generation.

## Tech Stack
- GitHub Pages (static hosting)
- Markdown (content via README.md)
- Optional: HTML/CSS/JS/Jekyll (for expansion)

## Key Files
- `README.md`: Core content; auto-rendered as index by GitHub Pages. **Read first.**

## Architecture
- **Root-level static site**: Single README.md serves as entrypoint.
- GitHub Pages flow: README.md → HTML render → Live site.
- Scalable to multi-file (index.html overrides README; _config.yml for Jekyll).

## Patterns & Conventions
- **Naming**: Kebab-case for files; semantic Markdown headers (e.g., `# Title`).
- **Structure**: Flat root; use `/assets/` for CSS/JS/images.
- **Markdown**: Standard GFM; no custom plugins yet.
- **Commits**: Descriptive messages (e.g., "Add homepage content").

## Common Tasks
- **Add feature** (e.g., new page): Create `index.html` or subdir (e.g., `/blog/index.md`); push to `main`.
- **Style site**: Add `assets/style.css`; link in HTML/Markdown.
- **Fix bugs**: Edit files locally; preview on GitHub or VS Code Live Preview; push.
- **Add Jekyll**: Create `_config.yml`; add layouts/posts; enable in repo Settings > Pages.
- **Deploy**: `git add . && git commit -m "Update" && git push`.

## Testing
- **Run locally**: Clone repo; open `README.md` in Markdown viewer (e.g., VS Code, Typora) or `npx serve .`.
- **Live preview**: Push to `main`; check https://mrspots1.github.io (updates ~1min).
- **Write tests**: None currently. Add via JS unit tests (Jest) or HTML validators (W3C).
  - Install: `npm init -y && npm i jest`.
  - Run: `npm test`.

## Important Notes
- **Gotchas**: README.md renders only if no `index.html`. GitHub ignores `.nojekyll` for plain static.
- **Quirks**: Case-sensitive paths; no server-side logic (static only).
- **Watch for**: Pages source must be `main` branch (Settings > Pages). Custom domain via DNS/CNAME.
- **Expand tip**: Fork Jekyll themes; `git submodule add` for deps.
```

*(Total: 48 lines. Optimized for quick AI parsing: scannable sections, action-oriented tasks.)*