# BobaBud website

Static site: `index.html` + `img/`, deployed by Netlify (`netlify.toml`, publish dir `.`, no build step).

## Deploy flow
Claude edits → push to a `claude/*` branch → GitHub Action `.github/workflows/claude-auto-deploy.yml`
merges it into `main` → Netlify deploys `main` to https://bobabud.netlify.app.

So after every tweak: commit and push your branch. Nothing else is needed for it to go live.
Keep `index.html` valid. Every push goes straight to production with no review.
