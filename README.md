# Sage Window Cleaning — Website

A single-page website for Sage Window Cleaning in Hamilton, Montana.
Everything lives in one file: `index.html` (no build step, no dependencies).

## Live site

The site is deployed with GitHub Pages at:
**https://almapowell.github.io/project1/**

Pushing changes to the site files automatically redeploys via the workflow in
`.github/workflows/deploy.yml` (it publishes the repo contents to the
`gh-pages` branch, which Pages serves).

## Preview it locally

Just open `index.html` in a browser, or serve the folder with any static host
(GitHub Pages, Netlify, Vercel, etc.).

## Swap in real photos

The "Recent Work" gallery currently uses illustrated placeholders. To use real
job photos:

1. Create an `images/` folder and drop the photos in it.
2. In `index.html`, find the `<section class="gallery" id="work">` block and
   replace each placeholder `<svg>...</svg>` inside a `<figure>` with:

   ```html
   <img src="images/your-photo.jpg" alt="Describe the job">
   ```

3. Update the `<figcaption>` text to describe each job.

## Other quick edits

- **Phone number** — search for `406-381-2496` / `+14063812496` and update everywhere.
- **Facebook link** — in the footer, replace `https://www.facebook.com/` with the
  page's real URL.
- **Service areas** — edit the list in the "Proudly serving" panel near the bottom.
- **Brand colors** — defined once as CSS variables at the top of the `<style>` block.
