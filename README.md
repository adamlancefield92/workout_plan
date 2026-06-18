# Home Split

A personal strength & power workout app (Legs / Push / Pull) with a built-in rest timer.
Single static page — no build step, no dependencies.

## Files
- `index.html` — the app (entry point)
- `apple-touch-icon.png` — iPhone Home Screen icon (180×180)
- `icon-192.png`, `icon-512.png` — larger icons (optional)

---

## One-time setup

### 1. Create the repo
1. On GitHub: **New repository** → name it `home-split` → **Public** → Create.
2. Add these files to the repo root: `index.html`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`.
   - Either drag them into the GitHub web uploader, or push with git (see below).

### 2. Turn on GitHub Pages
1. Repo → **Settings** → **Pages**.
2. **Source:** Deploy from a branch.
3. **Branch:** `main`, folder `/ (root)` → **Save**.
4. Wait ~1 minute. Your URL appears at the top:
   `https://<your-username>.github.io/home-split/`

### 3. Add to iPhone Home Screen
1. Open that URL in **Safari** (must be Safari, not Chrome).
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. It now opens full-screen like an app, with the dumbbell icon.

---

## Updating it (hands-off loop)

Ask **Claude Code** (pointed at this repo) to make a change. It will edit
`index.html`, then:

```bash
git add -A
git commit -m "Update workout"
git push
```

GitHub Pages redeploys in 30–60 seconds. Open the Home Screen icon and it's
updated — pull down to refresh if it ever looks stale.

> This repo is intentionally separate from the Hedgehog project.

### First-time git push (if not using the web uploader)
```bash
git init
git add -A
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/home-split.git
git push -u origin main
```
