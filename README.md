# Ayodele Mudavanhu: Portfolio

Static portfolio site (HTML + CSS + vanilla JS, no build step) for GitHub Pages.

```
index.html          page content
styles.css          design tokens, light/dark themes, layout
script.js           theme toggle, scroll reveal, project filters
assets/ayodele.jpg  profile photo
```

## Deploy to GitHub Pages

You already have the repo `Ayoworker/Ayoworker.github.io`, which serves https://ayoworker.github.io/.

1. Open https://github.com/Ayoworker/Ayoworker.github.io
2. Delete the old files (`index.html`, `styles.css`, `profile.jpg`, `project1-3.jpg`), or keep a copy in another branch first.
3. **Add file → Upload files**, then drag in `index.html`, `styles.css`, `script.js`, `README.md` and the `assets` folder.
4. Commit. After about a minute the new site is live at https://ayoworker.github.io/
5. If it doesn't update, check **Settings → Pages**: Source = "Deploy from a branch", Branch = `main`, folder `/ (root)`.

With git installed:

```bash
git clone https://github.com/Ayoworker/Ayoworker.github.io
# copy these files into the folder, replacing the old ones
git add -A
git commit -m "New portfolio"
git push
```

## Editing content

- **Text, projects and competitions** all live in `index.html`. Each project is an `<article class="card">` block. Copy one to add a project, and set `data-cat` to `ml`, `product` and/or `health` so the filter buttons work.
- **Colors and fonts** are the variables at the top of `styles.css` (`--color-accent` is the blue).
- **Zindi stats** in the highlights strip were taken from your public Zindi profile on 17 Nov 2026. Update them as your rank changes.

## Preview locally

```bash
python -m http.server 5173 --directory portfolio
```

Then open http://localhost:5173.
