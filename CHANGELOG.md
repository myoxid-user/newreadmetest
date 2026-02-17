# Changelog

## 2025-02-17

- Removed Supabase: deleted client and types, dependency, and env vars (was unused).
- Base path for deploy: Vite `base: "./"` and Router `basename` from `window.location`; no .env needed for GitHub Pages.
- GitHub Actions workflow added: build on push to `main` and deploy `dist` to GitHub Pages (use Settings → Pages → Source: GitHub Actions).
- Workflow: use `npm install` (not `npm ci`) and add Verify dist step for CI logs.
- Removed all Lovable branding: README, index meta, author; og/twitter image now local (placeholder.svg); dropped lovable-tagger from Vite and package.json.
- Fixed GitHub Pages links: resume PDF and 404 home link use relative/base-aware paths (./resume.pdf, Link to="/").
