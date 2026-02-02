# SETUP.md

## Overview

MrSpots1.github.io is a static website hosted on GitHub Pages, built using Markdown files. No build system or server-side dependencies are required. The site is automatically generated and deployed by GitHub from the repository's main branch.

## 1. Prerequisites

- **Git**: Version 2.30.0 or higher (for cloning and pushing changes).
- **GitHub Account**: Required for forking, contributing, or deploying via GitHub Pages.
- **Web Browser**: Any modern browser (e.g., Chrome 90+, Firefox 90+, Safari 14+) for previewing the site.
- **Markdown Editor**: Optional but recommended (e.g., VS Code, Typora).

No Node.js, Ruby, Python, or other runtimes are required.

## 2. Quick Start

1. Fork or clone the repository: `git clone https://github.com/MrSpots1/MrSpots1.github.io.git`.
2. Open `README.md` (or other `.md` files) in a Markdown editor or browser.
3. Edit Markdown files as needed.
4. Commit and push changes: `git add . && git commit -m "Update content" && git push origin main`.
5. View the live site at https://mrspots1.github.io (updates propagate in ~1-5 minutes).

## 3. Detailed Installation

### Clone Repository
```bash
git clone https://github.com/MrSpots1/MrSpots1.github.io.git
cd MrSpots1.github.io
```

### Install Dependencies
No dependencies or package managers are required. The site uses native GitHub Markdown rendering.

### Environment Setup
No environment variables or `.env` files are used. No `.env.example` exists.

### Database Setup
Not applicable. This is a static site with no database.

## 4. Running the Application

### Development Mode
1. Clone the repository (see above).
2. Open `README.md` or `index.md` (if present) in a Markdown viewer:
   - Browser: Drag-and-drop the file into Chrome/Firefox.
   - Local server (optional): Use `npx serve .` (requires Node.js) or Python's `python -m http.server`.
3. Changes to Markdown files are viewable immediately in the browser or editor preview.

### Production Mode
Push changes to the `main` branch:
```bash
git add .
git commit -m "Deploy updates"
git push origin main
```
GitHub Pages automatically builds and deploys from the `main` branch root. Site is live at https://mrspots1.github.io.

### With Docker
Not applicable. No Docker configuration exists.

## 5. Running Tests

Not applicable. No test suite or testing framework is present in the codebase.

## 6. Troubleshooting

| Issue | Possible Cause | Solution |
|-------|----------------|----------|
| Site not updating after push | GitHub Pages cache/delay | Wait 1-5 minutes; hard-refresh browser (Ctrl+Shift+R). Check Actions tab for build status. |
| Markdown not rendering correctly | Invalid Markdown syntax | Validate syntax using a linter like `markdownlint`. Ensure no broken links. |
| 404 on custom pages | File not in root or wrong branch | Confirm files are in `main` branch root. GitHub Pages serves from `/docs` folder only if configured (not here). |
| Clone fails | No Git installed or network issue | Install Git; check internet/proxy settings. |
| Local preview broken | Browser security blocking local files | Use a local server like `npx serve` or `python -m http.server`. |

For GitHub Pages-specific issues, refer to [GitHub Pages docs](https://docs.github.com/en/pages).

## 7. IDE Setup

### Recommended IDE: Visual Studio Code
Install these extensions for optimal Markdown/GitHub Pages development:

| Extension | Publisher | Purpose |
|-----------|-----------|---------|
| Markdown All in One | Yu Zhang | Preview, linting, auto-complete for Markdown. |
| GitHub Pull Requests and Issues | GitHub | Manage PRs/issues directly in VS Code. |
| Markdownlint | David Anson | Enforce Markdown style and catch errors. |
| GitLens | GitKraken | Enhanced Git blame/history visualization. |
| Live Server | Ritwick Dey | Local server for static previews (with live reload). |

1. Install VS Code: https://code.visualstudio.com/.
2. Open the cloned repo folder in VS Code: `File > Open Folder`.
3. Install extensions via the Extensions view (Ctrl+Shift+X).
4. Use Ctrl+Shift+V for Markdown preview.