# Aletheis Technologies website

Static website (one page, no build step). Open `index.html` in a browser to preview.

## Publish with GitHub Pages
1. Create a new repository on GitHub (for example `aletheis-website`).
2. Upload everything in this folder (`index.html`, `favicon.ico`, `.nojekyll`, `images/`) to the repository root.
3. In the repository go to **Settings → Pages**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, and save.
4. After a minute the site is live at `https://<your-username>.github.io/aletheis-website/`.

To use your own domain, add it under **Settings → Pages → Custom domain** and point your domain's DNS to GitHub Pages.

## Before going live
- Replace the dummy email `sales@aletheis.example` in `index.html` (search for it; it appears a few times).
- The quote form opens the visitor's email app. To collect requests without email, connect the form to a form service later.
