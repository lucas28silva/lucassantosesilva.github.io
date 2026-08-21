# lucas-santos-e-silva.github.io

Personal research site for Lucas Santos e Silva — PhD Candidate in Economics,
Universidade de Brasília.

## Structure

```
index.html        Home / About
research.html      Working papers, publications, conference proceedings
cv.html            Education & experience
contact.html        Contact / scholarly IDs
assets/style.css     All styling (single stylesheet, no build step)
```

No build tools, frameworks, or dependencies — just static HTML/CSS. Fonts are
loaded from Google Fonts via CDN link tags in each page's `<head>`.

## Before you publish

1. **Replace the placeholder email** in `contact.html` (currently
   `lucas.silva@example.com`).
2. Double-check the working paper entries in `research.html` — add short
   abstracts whenever you're ready to share more than the title.
3. If you want a downloadable CV, drop a `cv.pdf` into `assets/` and
   uncomment the download link at the top of `cv.html`.
4. Add a photo later, if you want one — none of the layouts require it, so
   it can be dropped in without breaking anything.

## Publishing to GitHub Pages

1. Create a new GitHub repository. For a personal top-level domain like
   `https://<username>.github.io`, name the repo exactly
   `<your-github-username>.github.io`. Otherwise, any repo name works and the
   site will be published at `https://<username>.github.io/<repo-name>/`.
2. Push these files to the repository's default branch (`main`):
   ```bash
   cd site
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**, and under "Build and
   deployment", set **Source** to "Deploy from a branch", branch `main`,
   folder `/ (root)`. Save.
4. GitHub will publish the site within a minute or two, at the URL shown on
   that same settings page.

## Custom domain (optional)

If you buy a domain later, add a `CNAME` file at the repo root containing
just your domain (e.g. `lucassantos.com`), then point your domain's DNS to
GitHub Pages per
[GitHub's custom-domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
