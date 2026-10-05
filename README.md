# GAC Residence V1

A responsive, static HTML/CSS/vanilla JavaScript landing site for GAC Residence. The page is organized into clear sections so the design and content can later move into reusable components and a Next.js application.

## Run locally

No build step or package install is required. Open `index.html` directly in a modern browser, or serve this folder with any static file server. For example, from this folder run `python -m http.server 8000` and visit `http://localhost:8000`.

## Project files

- `index.html` — content and page structure
- `styles.css` — responsive styling, layout and visual effects
- `script.js` — mobile menu, scroll state and reveal effects

## Before publishing

- Replace the cinematic hero placeholder with the client’s homepage video and add GAC-approved property photography in `styles.css`.
- Confirm the current Airbnb listing URLs and add the preferred direct contact details.
- The residence edit and host academy are presented as brand sections; add confirmed product/course details when available.

The live reference site was not accessible from the project runtime. Property names, locations and described amenities are based on publicly indexed GAC Residence Airbnb listings. Images are remote Unsplash placeholders and therefore need an internet connection until replaced with local approved assets.

## Preview hosting

This is a plain static site with no build command. Vercel is the fastest preview route here because it can deploy this folder directly, without setting up a GitHub repository. From this folder, run `npx vercel`, follow the first-time login/setup prompts, and share the preview URL it returns. When the client is ready for a production deployment, run `npx vercel --prod`. The `.vercelignore` file keeps project instructions and reference files out of the upload.

GitHub Pages is a good alternative if you want the site maintained in a GitHub repository. It requires a repository and Pages setup; see [GitHub Pages setup](https://docs.github.com/en/pages/getting-started-with-github-pages). For Vercel's deployment behavior, see [the Vercel CLI guide](https://vercel.com/docs/cli/deploy).

### GitHub Pages setup

1. Create a repository and clone it locally.
2. Copy `index.html`, `styles.css`, `script.js`, `README.md`, and `.nojekyll` into the cloned repository. Do not copy the `sources/` reference folder or project-only instruction files.
3. Commit and push the files to the repository's `main` branch.
4. In the repository, open **Settings → Pages** and choose **Deploy from a branch**, branch `main`, folder `/(root)`, then save.
5. Wait for the Pages deployment to finish; GitHub will show the published URL in the Pages settings.

GitHub Pages sites are public on the internet. With GitHub Free, the repository must also be public. Avoid putting private client details or payment secrets in the repository.
