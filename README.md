# Sanaullah Khan — Portfolio

Plain HTML/CSS/JS. No build tools, no framework, nothing to install. That
means the free Vercel deploy is very simple.

## Files
- `index.html` — all the content/text lives here
- `styles.css` — all the colors/spacing/design
- `script.js` — a small scroll-reveal effect (optional, page works without it)
- `assets/` — your images and CV PDF

## Editing content (in Cursor)
Open this folder in Cursor. Almost everything you'd want to change is plain
text inside `index.html` — headline, bio, job history, links, email, phone.
Search (Cmd/Ctrl+F) for the text you want to change and edit it directly. No
code needs to be understood to do this.

To swap the CV file: replace `assets/Sanaullah-Khan-CV.pdf` with your own
file of the same name (or update the filename in the "Download CV" button
in `index.html`).

## Deploy to Vercel for free (no coding)

**Step 1 — Put the folder on GitHub**
1. Go to https://github.com and create a free account if you don't have one.
2. Click the **+** in the top right → **New repository**. Name it e.g.
   `portfolio`. Leave it public. Click **Create repository**.
3. On the new repo's page, click **uploading an existing file** and drag
   this whole folder's contents in (index.html, styles.css, script.js, and
   the assets folder). Commit the changes.

   (If you'd rather do it from Cursor: open the folder in Cursor, open its
   built-in terminal, and run:
   ```
   git init
   git add .
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
   git push -u origin main
   ```
   replacing the URL with the one GitHub shows you after creating the repo.)

**Step 2 — Import it into Vercel**
1. Go to https://vercel.com and sign up free with your GitHub account.
2. Click **Add New → Project**.
3. Select the `portfolio` repository you just created.
4. Framework Preset: choose **Other**. Leave Build Command and Output
   Directory blank — there's nothing to build.
5. Click **Deploy**.

That's it. Vercel gives you a free URL like `portfolio-yourname.vercel.app`
within about a minute. Any time you push a new change to GitHub, Vercel
redeploys automatically.

**Optional: custom domain.** In the Vercel project → Settings → Domains,
you can attach a domain you own for free (you'd still pay whoever you buy
the domain from, e.g. Namecheap — Vercel's hosting itself stays free).
