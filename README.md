# GitHub Pages Staging

This folder is a dedicated publishing surface for frozen outputs that must not be rebuilt.

Current preserved exports:
- `01-05-2026__13-47-45`
- `01-05-2026__14-12-51`

Intent:
- keep the original builder outputs in `exports/` untouched
- copy the frozen outputs into `github_pages/`
- publish this folder through GitHub Pages

Suggested GitHub setup:
1. Create a dedicated GitHub repository for frozen outputs.
2. Copy the contents of this `github_pages/` folder into the root of that repo.
3. Push the repo to GitHub.
4. In GitHub:
   - go to `Settings`
   - open `Pages`
   - set the source to `Deploy from a branch`
   - choose the main branch and `/ (root)`
5. Wait for GitHub Pages to publish.

Expected landing page:
- root `index.html` links to both frozen export folders

Notes:
- each frozen output folder has its own `index.html` and `board.html`
- these copies are intended to remain verbatim publishing copies, separate from future builder runs
