# Publish Rental Property Management OS live

## Live URL
https://valensfinancial-arch.github.io/valens-rental-os/

Repo: https://github.com/valensfinancial-arch/valens-rental-os

GitHub Pages deploys from `main` via `.github/workflows/pages.yml`.

## Update from Grok
1. Tell Grok what to change.
2. Grok edits `index.html` and pushes to this repo.
3. Pages rebuilds; the live URL stays the same.
4. Browser `localStorage` on that origin is kept. Use header export/import for backups.

## Manual fallback
Drag this folder onto https://app.netlify.com/drop for a `*.netlify.app` URL.
