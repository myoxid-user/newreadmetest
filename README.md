# dibbed

Portfolio / resume site — Vite, TypeScript, React, shadcn-ui, Tailwind CSS.

## Run locally

```sh
git clone <YOUR_GIT_URL>
cd <PROJECT_DIR>
npm i
npm run dev
```

## Scripts

- `npm run dev` — dev server
- `npm run build` — production build
- `npm run preview` — preview production build
- `npm run lint` — ESLint
- `npm run test` — Vitest

## Deploy (GitHub Pages)

1. **Settings → Pages → Build and deployment → Source** → **GitHub Actions** (not "Deploy from a branch").
2. Push to `main`; the workflow builds and deploys. Site: `https://<user>.github.io/<repo>/`.

If the site shows a blank page or 404 for `/src/main.tsx`, the source is still "Deploy from a branch". Switch it to **GitHub Actions** in the repo Settings.

### Resume PDF (Download CV)

Put your resume in the repo so "Download CV" works and `https://<user>.github.io/<repo>/resume.pdf` opens:

```sh
# Copy your PDF into public/ as resume.pdf, then:
git add public/resume.pdf
git commit -m "Add resume PDF"
git push origin main
```

After the next deploy, the link and direct URL will work.

## Stack

- Vite, TypeScript, React
- shadcn-ui, Tailwind CSS
- Framer Motion, React Router, TanStack Query
