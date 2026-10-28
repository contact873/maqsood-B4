# M.RAIKOU website: the site before the proposal

A static site. No build step, no framework, no server. Every page is hand-written or generated HTML and
one stylesheet.

## Deploy to Vercel from GitHub

1. Create a repository and push these files so that **`index.html` is at the repository root**.
2. On vercel.com choose **Add New → Project** and import the repository.
3. Framework preset: **Other**. Build command: **none**. Output directory: **leave empty** (the root is
   the site). No `vercel.json` is needed.
4. Deploy. `index.html` serves at `/`, and `cars-auto-parts/index.html` serves at `/cars-auto-parts/`.

## What is in the bundle

- `index.html` — English
- `ur.html` — Urdu
- `ja.html` — Japanese
- `ar.html` — Arabic
- `websites.html`, `websites-ja.html` — the website-building page for M.RAIKOU's clients
- `assets/style.css` — the single stylesheet for every page

- `cars-auto-parts/` is **not** in this bundle; the car pages come with the proposal.

## Two things to know

- **Canonical URLs point at `https://mraikou.com/`.** On a Vercel preview domain they still will. That is
  deliberate while this is a replacement for the live site; change them if the preview should be indexed
  instead.
- **The forms have no server.** Each one composes an email or a WhatsApp message from the visitor's own
  phone, which is why they work on a host with no backend.

