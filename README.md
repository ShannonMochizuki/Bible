# Journey Through Joshua — upload-ready GitHub Pages build

This folder is designed to be uploaded directly to the root of a GitHub repository. No build step is required.

## Files to upload
Upload **all files in this folder** to the repository root, so `index.html` is at the top level. Do not upload the ZIP itself to GitHub Pages.

Required:
- `index.html` — the complete app (CSS, Joshua 1–4 content, and app logic are embedded)
- `manifest.webmanifest` — PWA manifest
- `sw.js` — offline cache / update handling
- `icon.svg`, `icon-192.png`, `icon-512.png` — app icons
- `.nojekyll` — tells GitHub Pages to serve the static files directly

## GitHub Pages
1. Create or open the repository you want to use.
2. Choose **Add file → Upload files**.
3. Upload the files above to the repository root and commit them.
4. In **Settings → Pages**, choose **Deploy from a branch**.
5. Select the branch containing these files (normally `main`) and folder `/ (root)`. Save.
6. Wait for GitHub Pages to finish deployment, then refresh the site.

The app uses only relative paths, so it works both at `username.github.io` and at `username.github.io/repository-name/`.

## If an older broken version is cached
The v2 service worker removes older app caches. After deployment, refresh the page once. If a browser still shows the old page, close the tab and reopen the site.

## NKJV note
The app is designed for NKJV study but does not redistribute the full copyrighted NKJV text. It uses passage references, study prompts, and explanatory material. Licensed NKJV text can be added later.
