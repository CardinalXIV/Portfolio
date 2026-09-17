# Benaiah Mark Mo Di — Portfolio Site

A single-page portfolio built with plain HTML/CSS/JS (no build step, no dependencies) using an iOS-style "liquid glass" design. Ready to host for free on GitHub Pages.

## Files

- `index.html` — the entire site (structure, styles, and interactivity all in one file)
- `assets/Benaiah_Mark_Mo_Di_Resume.pdf` — downloadable resume, linked from the "Download Resume" buttons

## Deploy to GitHub Pages (free)

You have two options. Option A gives you a URL like `https://CardinalXIV.github.io`. Option B gives you a URL like `https://CardinalXIV.github.io/portfolio`.

### Option A — your main GitHub Pages site (recommended)

1. On GitHub, create a **new repository** named exactly: `CardinalXIV.github.io`
   (it must match your GitHub username exactly, all lowercase is fine too)
2. Do not initialize it with a README (or if you do, you'll just overwrite it in step 4).
3. On your computer, unzip this folder, then run:
   ```bash
   cd portfolio-site
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/CardinalXIV/CardinalXIV.github.io.git
   git push -u origin main
   ```
4. Go to the repo on GitHub → **Settings → Pages**. Under "Build and deployment", make sure Source is set to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
5. Wait 1–2 minutes, then visit **https://CardinalXIV.github.io** — your site is live.

### Option B — a project site under any repo name

1. Create a repo with any name, e.g. `portfolio`.
2. Push these files to it the same way as steps 3 above, but with that repo's URL as the remote.
3. In **Settings → Pages**, set Source to `main` branch, `/ (root)` folder.
4. Your site will be live at **https://CardinalXIV.github.io/portfolio**.

## Making changes later

Just edit `index.html` directly (it's plain HTML/CSS/JS — search for the section you want, e.g. `id="projects"`), commit, and push. GitHub Pages redeploys automatically within a minute or two.

To swap in a newer resume, replace `assets/Benaiah_Mark_Mo_Di_Resume.pdf` with your new PDF (keep the same filename, or update the two `href` links in `index.html` that point to it).

## Notes

- The site includes a light/dark mode toggle (top right) and is fully responsive down to phone widths.
- Phone number was intentionally left off the public page to reduce spam exposure — it's still on the downloadable resume PDF. Add it back near the email link in the `#contact` section if you'd like it visible.
- Three project links you mentioned (AuditSense, CSC3109Grp02, DataAnalyticsCSC3105) returned 404s when checked — likely private repos or renamed. Make them public (or fix the repo name) and I can wire them into the "Academic & Personal" grid, or just add them yourself following the existing `.mini-card` pattern in `index.html`.
