# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Install dependencies
bundle install

# Local development server with live reload (http://localhost:4000)
bundle exec jekyll serve --livereload

# Build static site
bundle exec jekyll build --safe

# HTML validation (run after build)
bundle exec htmlproofer ./_site --disable-external --check-html --allow-hash-href
```

## Architecture

This is a **Jekyll static site** (personal portfolio + French-language technical blog) hosted on GitHub Pages.

### Content Collections

- `_posts/` — Blog articles, named `YYYY-MM-DD-title.md`
- `_projects/` — Portfolio project pages
- Static pages: `index.html`, `about.md`, `blog.md`, `skills.md`, `contact.md`, `projects.md`

### Layout System

- `_layouts/default.html` — Base layout (header, nav, footer)
- `_layouts/post.html` — Blog post with sharing buttons and prev/next navigation
- `_layouts/project.html` — Project showcase
- `_layouts/archive-*.html` — Tag and year archive pages

### Styling

SCSS partials in `_sass/`:
- `_variables.scss` — Colors, spacing, breakpoints, typography (edit this for theme changes)
- `_base.scss`, `_layout.scss`, `_components.scss`, `_utilities.scss`

Key design tokens:
- Primary: `#2563eb`, Secondary: `#64748b`, Accent: `#f59e0b`
- Breakpoints: 640px, 768px, 1024px, 1280px
- Font: Inter

### Data Files (`_data/`)

- `site.yml` — Site metadata and navigation structure
- `theme.yml` — Theme color and typography variables
- `posts.yml` — Post metadata defaults and social sharing config

### CI/CD

GitHub Actions (`.github/workflows/jekyll.yml`) builds and deploys on push to `main`:
1. Setup Ruby 3.1
2. `bundle exec jekyll build --safe`
3. HTMLProofer validation
4. Deploy via `peaceiris/actions-gh-pages@v3`

### Key Plugins

`jekyll-feed`, `jekyll-sitemap`, `jekyll-seo-tag`, `jekyll-paginate` (5 posts/page), `jekyll-archives` (year + tag archives), `jekyll-admin` (dev only)

### JavaScript

Vanilla JS only — mobile nav toggle, smooth scrolling, scroll-triggered header effects. No frameworks.
