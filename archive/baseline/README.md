# GitHub Pages Publish Surface

This folder now publishes the promoted enriched frozen outputs.

Active behavior:
- enriched `index.html` / `board.html` inside each frozen run folder
- root `index.html` is the promoted review hub
- baseline pre-promotion surface is preserved under `archive/baseline/`

Maintenance notes:
- rebuild local validation from the untouched baseline logic first if needed
- only promote after the enriched clone and validation report are satisfactory
- `github_pages/.git` remains the publishing repo metadata and is not touched by builder exports
