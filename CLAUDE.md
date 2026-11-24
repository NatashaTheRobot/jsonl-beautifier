# JSONL Beautifier

A static site: `index.html` is the whole app.

## Deploy

- GitHub Pages publishes the `main` branch root to jsonlbeautifier.com. Every push to `main` goes live; there is no staging.

## Working rules

- Every committed file is served publicly at jsonlbeautifier.com/<path>. Keep plans, drafts, screenshots and renders out of the repo.
- `index.md` and `llms.txt` restate the page's features and limits (25 records per page, the 1 MB large-file mode, the accepted file types, no third-party scripts or trackers). Change them in the same commit as `index.html`.
