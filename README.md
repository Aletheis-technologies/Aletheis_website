# Aletheis Technologies Website

Marketing website for Aletheis Technologies and the **AL-WCT-1002 Wireless Communication Trainer**. The site presents the product, its Windows software, included antennas, lab experiments, specifications, and a quote-request flow.

## Live website

Visit the published site at **[aletheis-technologies.github.io/Aletheis_website](https://aletheis-technologies.github.io/Aletheis_website/)**.

## Features

- Responsive, single-page static website
- Tabbed sections for Home, Product, How it works, About us, and Quote
- Product detail sub-tabs for software, antennas, kit contents, experiments, and specifications
- Light and dark themes
- Animated signal rings and oscilloscope-style visualizations using HTML Canvas
- Reduced-motion support through `prefers-reduced-motion`
- Accessible labels, focus styles, and semantic navigation controls
- Quote form that opens the visitor's email application with a pre-filled request
- No frontend framework, build step, or package manager required

## Project structure

```text
.
├── index.html       # Complete site markup, styles, and client-side behavior
├── favicon.ico      # Browser fallback favicon
├── .nojekyll        # Prevents GitHub Pages from running Jekyll
└── images/          # Product photography, logos, icons, and UI screenshots
```

## Deployment

The site is currently deployed to GitHub Pages at [aletheis-technologies.github.io/Aletheis_website](https://aletheis-technologies.github.io/Aletheis_website/). It can also be deployed to any static hosting provider, including Netlify or Vercel. Publish the repository root and use `index.html` as the entry point. No build command or environment variables are required.

For GitHub Pages:

1. Open the repository's **Settings → Pages**.
2. Select the branch and the repository root as the source.
3. Save the configuration and wait for the deployment to finish.

The included `.nojekyll` file ensures that the static files are served as-is.

## Editing content

Most site content is intentionally kept in `index.html`:

- Update headings, copy, product details, and navigation labels in the HTML.
- Update colors, typography, layout, and responsive styles in the `<style>` block.
- Update interactions and animations in the `<script>` block.
- Replace or add media in `images/`, then update the corresponding `src` and `alt` attributes.

The quote form currently sends requests to `sales@aletheis.example` through the visitor's default email client. Replace this address in the quote-form script before production use.

The page loads Archivo, IBM Plex Sans, and IBM Plex Mono from Google Fonts. If the site must work without third-party requests, self-host those fonts and update the font declarations in `index.html`.

## Browser support

The site is designed for current desktop and mobile browsers with support for modern CSS, Canvas, and standard browser APIs such as `history`, `matchMedia`, and `navigator.clipboard`. A fallback selection behavior is included for browsers that do not allow clipboard access.

## License

No license file is currently included. Add a license before redistributing the website or its assets.
