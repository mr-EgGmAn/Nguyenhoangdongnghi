# Nguyen Hoang Dong Nghi — CV website

Responsive personal CV website for Nguyen Hoang Dong Nghi, Data Analyst and
Business Analyst.

## Local preview

Because this is a static site, serve the repository root with any static HTTP
server. For example, with Node.js:

```powershell
npx --yes serve .
```

Then open the local URL printed by the command. Opening `index.html` directly
also works for the core page, but an HTTP server provides the closest match to
GitHub Pages.

## Project structure

```text
index.html                 Main page and CV content
styles.css                 Responsive layout, print styles, and theme
script.js                  Accessible mobile navigation
assets/CV_NGHI.pdf         Downloadable source CV
.github/workflows/         GitHub Pages deployment workflow
```

## GitHub Pages deployment

The workflow in
`.github/workflows/deploy-pages.yml` deploys automatically when changes are
pushed to `main`. It can also be started manually from the **Actions** tab.

For a repository-level Pages setup:

1. Open **Settings → Pages** on GitHub.
2. Set **Source** to **GitHub Actions**.
3. Push to `main` and monitor the **Deploy static site to GitHub Pages**
   workflow.

The expected project URL is:
`https://mr-eggman.github.io/Nguyenhoangdongnghi/`

## Content notes

The website content is based on `doc/CV_NGHI.pdf`. The original PDF is copied
to `assets/CV_NGHI.pdf` so visitors can download it without exposing the
source-document directory structure.
