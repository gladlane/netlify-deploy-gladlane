# Gladlane website

Static site for gladlane.com — landing page plus legal pages.

## Files

```
index.html                        Landing page
privacy.html                      Privacy Policy
terms.html                        Terms & Conditions
data-processing-addendum.html     Data Processing Addendum (DPA)
```

All pages are self-contained (HTML + inline CSS, fonts loaded from Google Fonts). No build step required.

## Editing the legal pages

The three legal pages were generated from Markdown source. If you keep editing in HTML directly, that's fine. If you'd rather keep a Markdown source of truth, the originals are kept alongside this repo and re-exported to HTML when changed.

## Deploy

### Netlify
Drag the whole folder onto the Netlify deploy area (or connect this GitHub repo to a Netlify site). Netlify serves `index.html` as the homepage; the other pages are reachable at `/privacy.html`, `/terms.html`, and `/data-processing-addendum.html`.

### GitHub Pages
Push to GitHub, then enable Pages on the repo (Settings → Pages → deploy from branch). The footer links are relative, so the site works whether it's served from a custom domain or a `username.github.io/repo` subpath.

## Links

The footer on every page links to Privacy, Terms, and DPA. "Security" is a placeholder (`#`) and "Contact" is a `mailto:` to security@gladlane.com — update these when you have dedicated pages/addresses.

## Before going live

- Publish a real DPA at the path the Terms reference (this repo includes it as `data-processing-addendum.html`).
- Confirm every factual claim in the policies is true (e.g. encryption at rest, the security measures listed, the AI no-training commitment per provider).
- Have the documents reviewed by a lawyer, especially the payments and sub-processor sections.
