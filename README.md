# Parallelism Atlas

An interactive guide to 18 transformer parallelism techniques and variants. Explore which weights, tokens and model states each GPU owns, and step through computation and communication.

The site is plain HTML, CSS and JavaScript in `dist/`; no package installation or build is required. All asset URLs are relative, so it supports GitHub Pages project URLs.

## Local preview

Run `python3 -m http.server 8000 --directory dist` and open http://localhost:8000.

## GitHub Pages

1. In repository Settings → Pages, choose **GitHub Actions** as the source.
2. Push to `main`, or run **Deploy Parallelism Atlas to GitHub Pages** from the Actions tab.
3. The deployment job reports the published URL. Subsequent pushes to `main` redeploy automatically.

Only `dist/` is deployed. GitHub's built-in workflow token handles deployment; no personal token or deployment secret is needed.

## Editing

- `dist/index.html`: page structure
- `dist/style.css`: styles and responsive layout
- `dist/app.js`: technique explanations, primary sources, diagrams and interactions

Diagrams are conceptual illustrations, not performance simulations. Ambiguous terminology and implementation assumptions are noted in the interface.
