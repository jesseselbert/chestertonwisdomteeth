# Deploying to Cloudflare Pages

## Recommended setup

- Host this folder as a static site on Cloudflare Pages.
- Keep `GlacialSandsOMS.com` as the main practice site.
- Point `chestertonwisdomteeth.com` to the new Pages project.

## Basic steps

1. Put the contents of this folder in a GitHub repo, or a subfolder connected to GitHub.
2. In Cloudflare, go to **Workers & Pages** and create a new **Pages** project.
3. Connect the repo.
4. Set the build configuration to:
   - Framework preset: `None`
   - Build command: leave blank
   - Build output directory: `/`
5. After deploy, add the custom domain `chestertonwisdomteeth.com`.
6. If desired, also add `www.chestertonwisdomteeth.com` and redirect it to the root domain.

## Important note on URLs

These pages are currently file-based:

- `dentist-vs-oral-surgeon.html`
- `wisdom-teeth-removal-chesterton-in.html`
- etc.

If you want perfectly clean URLs without `.html`, the next step is either:

- convert each page into a folder with an `index.html`, or
- add Cloudflare routing rules during deployment.

## Suggested next content wave

- `iv-sedation-wisdom-teeth-chesterton-in`
- `emergency-tooth-extraction-chesterton-in`
- `tooth-transplantation-chesterton-in`
- `wisdom-teeth-removal-la-porte-in`
- `northwest-indiana-wisdom-teeth-removal`
