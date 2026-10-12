# Youssof Ahmed Aly — Portfolio

A two-page portfolio site: `index.html` (home) and `projects.html` (all projects). Each page has its CSS and JavaScript inline, with no build step.
Fonts load from Google Fonts. Six colour themes are built in (default: Dusk) and the visitor's choice is remembered in the browser.

## Files
- `index.html` — home page
- `projects.html` — all 9 projects, each expandable
- `Youssof_Ahmed_Aly_CV.pdf` — one-page CV (the "Download CV" button)
- `Youssof_Ahmed_Aly_CV_full.pdf` — two-page CV
- `.nojekyll` — tells GitHub Pages to serve the files as they are

The CV files here have no phone number, because they are public. Keep the versions with your phone number for job applications.

## Deploy with GitHub Pages
1. Create a repository named `Dolphiny-1412.github.io` (the site is then served at `https://dolphiny-1412.github.io/`).
2. Upload all six files to the `main` branch, keeping the file names exactly as they are.
3. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then save.

## Page order
Home page: About (summary) → Education → Experience → Skills → Projects (3 featured) → Contact. The full list of projects is on `projects.html`.

## Adding a project
In `projects.html`, search for `class="arc"`. Copy one whole `<details class="arc" ...> ... </details>` block, paste it in the list, then change:
- `id` and `data-cat` — `data-cat` is one of `cyber`, `ml`, `systems`, `games`
- the code (`P.10`), title, one-line summary and category label in the `<summary>`
- the text, key points, stack tags and link inside the block
Then update the number on the matching filter chip (search for `data-filter`).

## Changing the featured three
The three large cards on the home page are the `<article class="pcard">` blocks. Each has a "Full details" link to its row on `projects.html`.
