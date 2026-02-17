# Changelog

## 2025-02-17

- Removed Supabase: deleted client and types, dependency, and env vars (was unused).
- Base path for deploy: Vite `base: "./"` and Router `basename` from `window.location`; no .env needed for GitHub Pages.
- GitHub Actions workflow added: build on push to `main` and deploy `dist` to GitHub Pages (use Settings → Pages → Source: GitHub Actions).
