# masoudzp.github.io

Personal academic website, built by GitHub Pages with Jekyll. Push to `main` and GitHub rebuilds the site automatically; nothing needs to be installed locally.

## Editing

| What to change | File |
|---|---|
| Home page text (bio, research, section order) | `index.md` |
| Appointments, education, honors | `CV.md` |
| Group members | `people.md` |
| Any publication (all pages read from this one file) | `_data/publications.yml` |
| Colors, fonts, spacing | `assets/css/style.css` |
| Sidebar menu items | `nav:` in `_config.yml` |
| Page skeleton (sidebar + content) | `_layouts/default.html` |

### Adding a publication

Add an entry at the top of `_data/publications.yml`:

```yaml
- title: Paper title
  authors: First Author, Second Author, Masoud Zarepisheh
  venue: Medical Physics
  year: 2026
  url: https://doi.org/...
  links:            # optional; any label works
    arXiv: https://arxiv.org/abs/...
    Code: https://github.com/...
    Slides: /assets/my-slides.pdf
  selected: true    # optional: also show under "Selected publications" on the home page
  tag: Method · problem it addresses   # optional: shown on the home page only
```

The CV page groups entries by `year` automatically, in the order they appear in the file (keep it newest first). Put slide decks and other PDFs in `assets/`.

## Previewing locally (optional)

```
gem install jekyll jekyll-seo-tag jekyll-sitemap
jekyll serve
```

Then open <http://localhost:4000>.
