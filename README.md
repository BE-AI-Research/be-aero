# BE-Aero website

Static site for BE-Aero: `index.html` (home) and `guide.html` (guide and help). No build step, no dependencies. Every path is relative, so it works from any folder or domain.

## Publish on GitHub Pages

This folder is laid out for the `BE-AI-Research/sites` repository at `be-aero-apps/`.

1. Copy the contents of this folder into `be-aero-apps/` in the repository and push.
2. In the repository: **Settings > Pages > Build and deployment**. Source: **Deploy from a branch**. Branch: `main`, folder `/ (root)`. Save.
3. After a minute the site is at `https://be-ai-research.github.io/sites/be-aero-apps/`.

To serve it at the root of its own repository or a custom domain instead, put these files at the repository root, choose `/ (root)` as above, and add a `CNAME` file containing the domain (for example `aero.beairesearch.ca`). Then add a DNS CNAME record pointing that name to `be-ai-research.github.io`.

`.nojekyll` tells Pages to serve the files exactly as they are. `404.html` is shown for missing pages when the site is served from a repository root or custom domain.

## Files

- `index.html`, `guide.html`: the two pages
- `styles/be-aero.css`, `themes/themes.css`: the product's own styles and nine themes, from the marketing pack. Do not edit these here; replace them from the pack.
- `styles/site.css`: the site's layout, built on those styles
- `icons/`, `img/`: icons and screenshots (WebP)

## Before you publish

- The assistant screenshot (`img/agent-browser.webp`) shows a pizza order with a name and a street address.
- The BE-Aero Files source menu (`img/files-sources.webp`) shows the device names Shayne-DSKTP and Shayne Tablet.
- Release status on both pages: Desktop 1.2.9 and Relay 1.0.2 published, 1.3.0 built and not yet published. Update the chips and the "Get BE-Aero" table when 1.3.0 ships.
