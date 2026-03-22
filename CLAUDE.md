# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Install dependencies
npm install

# Local development server (http://localhost:4321)
npm run dev

# Build static site
npm run build

# Preview production build
npm run preview
```

## Architecture

This is an **Astro static site** (personal portfolio + French-language technical blog) hosted on **Cloudflare Pages**.

### Content Collections

- `src/content/blog/` — Blog articles (`slug.md` or `slug.mdx`)
- `src/content/projects/` — Portfolio project pages
- `src/content/config.ts` — Zod schemas for all collections

### Frontmatter schemas

**Blog posts:**
```yaml
---
title: "Article title"
description: "Short description"
date: 2026-01-15
tags: ["tag1", "tag2"]
draft: false          # optional, defaults to false
---
```

**Projects:**
```yaml
---
title: "Project name"
description: "Short description"
date: 2026-01-15
tags: ["React", "TypeScript"]
github: "https://github.com/..."   # optional
demo: "https://..."                 # optional
featured: false                     # optional
---
```

### Layout System

- `src/layouts/BaseLayout.astro` — Base layout (header, nav, footer, SEO)
- `src/layouts/BlogPost.astro` — Blog post with prev/next navigation
- `src/layouts/Project.astro` — Project showcase with links

### Pages

- `src/pages/index.astro` — Homepage
- `src/pages/blog/index.astro` — Blog listing
- `src/pages/blog/[slug].astro` — Individual post
- `src/pages/projects/index.astro` — Projects listing
- `src/pages/projects/[slug].astro` — Individual project
- `src/pages/tags/[tag].astro` — Tag archive
- `src/pages/about.astro`, `skills.astro`, `contact.astro`
- `src/pages/rss.xml.js` — RSS feed
- `src/pages/404.astro` — Not found

### Styling

Single SCSS file: `src/styles/global.scss`

Key design tokens (CSS custom properties):
- `--primary: #2563eb`
- `--secondary: #64748b`
- `--accent: #f59e0b`
- Font: Inter (Google Fonts)

### Deployment — Cloudflare Pages

Connect the GitHub repo at https://dash.cloudflare.com → Pages → Create a project

Build settings:
- Build command: `npm run build`
- Build output directory: `dist`
- Node version: `22`

GitHub Actions (`.github/workflows/ci.yml`) validates the build on every push.

### Key Dependencies

- `astro` ^4.16 — Static site generator
- `@astrojs/mdx` — MDX support for richer blog posts
- `@astrojs/sitemap` — Automatic sitemap generation
- `@astrojs/rss` — RSS feed generation
- `sass` — SCSS compilation
