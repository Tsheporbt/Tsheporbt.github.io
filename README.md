# Tshepo Rabotapi — Portfolio website

A responsive, editorial-style static portfolio for GitHub Pages. Built with plain HTML, CSS and JavaScript. No build tools, framework, package manager or paid hosting required.

## Files

- `index.html` — complete website content and page structure
- `styles.css` — responsive visual design
- `script.js` — mobile navigation, project filters and current year
- `favicon.svg` — site icon
- `robots.txt` and `sitemap.xml` — basic search-engine discovery files
- `404.html` — simple not-found page
- `config.yml` — minimal Jekyll metadata

## Before publishing

1. Check the personal details, role dates, qualification names and links in `index.html`.
2. Add a current CV if you want a downloadable CV link. No CV was supplied with this rebuild, so the website does not pretend one is available.
3. Check that the existing `assets/images/new.jpg` portrait is the photograph you want to use. This version uses an original typographic hero illustration, so the old portrait is not required for the layout.
4. The old `assets/` directory is deliberately not included in this package. Keep your existing `assets/` directory in the GitHub repository if you want to retain the original images and other files for future use. The new homepage does not depend on those old images.
5. Review the project summaries for confidentiality and confirm that institutional material is approved for public display.

## Publish to the existing GitHub Pages repository

The repository is `Tsheporbt/Tsheporbt.github.io`, so the expected website address is `https://tsheporbt.github.io/`.

### Option A — GitHub website (no command line)

1. Download and unzip this package.
2. Open the repository: https://github.com/Tsheporbt/Tsheporbt.github.io
3. Open `index.html`, select the pencil (Edit) button, replace the file contents with the new `index.html`, and commit the change.
4. Repeat for `styles.css`, `script.js`, `favicon.svg`, `robots.txt`, `sitemap.xml`, `404.html`, `config.yml` and `README.md`.
5. If GitHub asks whether to create a new file, choose that option for files that do not already exist.
6. Open **Settings → Pages** and check the publishing source. For a standard user site, publishing from `main` and `/(root)` is sufficient. Do not change a working deployment method unnecessarily.
7. Open `https://tsheporbt.github.io/` and hard-refresh with `Ctrl + Shift + R`.

### Option B — GitHub Desktop

1. Clone `https://github.com/Tsheporbt/Tsheporbt.github.io.git`.
2. Copy the contents of this package into the repository folder, replacing files with the same names. Keep the existing `assets/` folder.
3. Commit with the message `Rebuild portfolio with editorial layout`.
4. Push to `main`.
5. Wait for GitHub Pages to finish publishing, then check the live site.

### Option C — Git command line

Run these commands from a local clone of the repository after copying the package files into it:

```bash
git add index.html styles.css script.js favicon.svg robots.txt sitemap.xml 404.html config.yml README.md
git commit -m "Rebuild portfolio with editorial layout"
git push origin main
```

## Editing the content

Most content is in `index.html`. Search for the section heading or project title you want to change. Styling is in `styles.css`. Project filters use the `data-category` values `analytics`, `learning` and `machine-learning`.

## Important accuracy and privacy notes

- The website intentionally avoids invented publication titles, awards, testimonials, public dashboard links and performance claims.
- The teaching evaluation and student engagement work is described at a high level. Do not publish raw student data, staff information, internal dashboards or institutional screenshots without explicit approval.
- The portfolio includes only one direct project source link that was already present in the existing site: the MobileNetV2 fruit-classification repository.
- Confirm that your current job title, dates, qualifications and public contact details are still accurate before publishing.
- The email, LinkedIn, GitHub and X links are carried over from the existing portfolio.

## Local preview

You can open `index.html` directly in a browser. For a local server, run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.
