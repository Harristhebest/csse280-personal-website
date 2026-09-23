# CSSE280 — Personal Website

A personal website created for CSSE280 at Rose-Hulman Institute of Technology. It combines an introduction, a photography portfolio, and a résumé using plain HTML, CSS, and JavaScript.

## Pages

| Page | Purpose |
| --- | --- |
| [index.html](index.html) | About page introducing Harris Wu, engineering studies, travel, and photography |
| [portfolio.html](portfolio.html) | Photography gallery featuring landscapes, wildlife, and night skies |
| [resume.html](resume.html) | Education, technical skills, projects, and honors from the original course period |

The biography and résumé are historical project content. Dates, student status, and résumé entries should be reviewed before treating the site as a current professional profile.

## Preview locally

No framework, package manager, or build step is required. Open `index.html` directly in a browser, or serve the repository with Python:

```sh
git clone https://github.com/Harristhebest/csse280-personal-website.git
cd csse280-personal-website
python3 -m http.server 8000
```

On Windows, `py -m http.server 8000` is an alternative. Open <http://localhost:8000> and use the navigation links to move between the three pages. Stop the server with Ctrl+C.

## File layout

```text
.
├── index.html
├── portfolio.html
├── resume.html
├── images/           # Photos, icons, and supporting images
├── style/
│   ├── main.css      # Site styles
│   └── normalize.css
└── script/
    └── main.js       # Counter exercise script
```

## Editing the site

- Update the relevant HTML file for page content and navigation.
- Edit `style/main.css` for layout, typography, and colors.
- Add images under `images/` and reference them with relative URLs.
- Preview all three pages after changing shared styles or navigation.

## Current implementation notes

The README describes the files as they currently exist; the original page code has been preserved.

- All three HTML pages reference `sript/main.js`, while the actual directory is `script/`. The JavaScript is therefore not loaded from the intended path.
- `script/main.js` contains a counter exercise that expects elements named `#dec`, `#inc`, `#res`, and `#count`. Those controls are absent from the current pages, so simply correcting the script URL also requires guarding or removing the unused counter behavior.
- The photography page uses backslashes in some image paths. Forward slashes are the portable form for web URLs.
- `style/normalize.css` is currently empty.

These observations identify small follow-up fixes without implying that they have already been applied.

## Repository context

The original photos and page content remain part of the project. The repository was previously named `csse280_web_design` and is now named `csse280-personal-website`.
