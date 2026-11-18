# VYRGON website

Static site (HTML, CSS, JavaScript). No build step. Works on GitHub Pages.

## Files
- `index.html`  the whole website (hero with animated app mockups, how it works, app showcase, audiences, form, FAQ)
- `privacy.html`, `terms.html`  draft legal pages (fill in the highlighted [placeholders] and have a lawyer review)
- `assets/logo.svg`, `assets/favicon.svg`  logo and tab icon
- `CNAME`  your custom domain (vyrgon.com)
- `.nojekyll`  tells GitHub Pages to serve the files as they are

## Put it on GitHub Pages
1. Open your repo (Mjdesign2020/vyrgon-website) on github.com.
2. Add file > Upload files. Drag in everything from this folder, including the `assets` folder. Commit changes.
3. Settings > Pages: Source = Deploy from a branch, branch `main`, folder `/ (root)`. Custom domain `vyrgon.com`, tick Enforce HTTPS.
4. Wait 1 to 3 minutes and refresh vyrgon.com.

## Things to edit (all in the CONFIG block near the bottom of index.html)
- `FORM_ENDPOINT`: paste your Formspree (or similar) endpoint URL so the early-list form really sends. Until you do, the form honestly tells visitors nothing was sent.
- `PLATFORM_LINKS`: add the App Store / Google Play URLs when the app is published. The "Coming soon" badges turn into real links.
- `SOCIALS`: add your real social URLs; only filled ones appear in the footer.

## Replacing the preview app screens
The phone screens are drawn in code (search for `const SCREENS` in index.html) with sample names and content. When your designer's real screens are ready, replace them with images: put the PNGs in `assets/` and swap each screen's HTML for an `<img>`.
