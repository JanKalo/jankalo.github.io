# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Academic personal website for Jan-Christoph Kalo (Assistant Professor, UvA INDElab), built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme. Deployed to GitHub Pages via GitHub Actions on push to `main`.

## Development Commands

**Local development with Docker (recommended):**
```bash
docker compose up
```
Serves at `http://localhost:8080` with live reload. Auto-restarts Jekyll when `_config.yml` changes.

**Local development without Docker:**
```bash
bundle install
bundle exec jekyll serve --port 8080 --livereload
```
Requires Ruby, Bundler, and ImageMagick on PATH.

**Production build (what CI runs):**
```bash
JEKYLL_ENV=production bundle exec jekyll build
```
Output goes to `_site/`. CI also runs PurgeCSS (`purgecss -c purgecss.config.js`) on the built CSS.

**Prettier (for Liquid templates):**
```bash
npx prettier --check .
npx prettier --write .
```
Uses `@shopify/prettier-plugin-liquid`.

## Architecture

- **Theme:** al-folio (Jekyll). Layouts use Liquid templates (`.liquid` files in `_layouts/`, `_includes/`).
- **Content pages:** `_pages/*.md` — each page has YAML front matter with `layout`, `permalink`, `nav`, `nav_order`. Pages with `nav: true` appear in the navbar, ordered by `nav_order`.
- **Publications:** Managed via `_bibliography/papers.bib` (BibTeX) and rendered by `jekyll-scholar`. Add `selected={true}` to a bib entry to feature it on the homepage. The `_layouts/bib.liquid` template controls how each entry renders.
- **News items:** Markdown files in `_news/`. Shown on homepage when `announcements.enabled: true` in `_config.yml`.
- **Blog posts:** `_posts/` (currently unused, `latest_posts.enabled: false`).
- **Projects:** `_projects/` directory.
- **Data files:** `_data/` contains `coauthors.yml`, `cv.yml`, `repositories.yml`, `venues.yml`.
- **Styles:** SCSS in `_sass/`, with `_variables.scss` for theme customization.
- **Custom plugins:** Ruby plugins in `_plugins/` (citation badges, cache busting, external posts, etc.).

## Key Configuration

All site-wide settings live in `_config.yml`. Important sections:
- Personal info (name, email, social links) at the top
- `scholar:` block controls bibliography rendering (style, grouping, author highlighting)
- `collections:` defines `news` and `projects`
- `imagemagick:` for responsive WebP image generation (requires ImageMagick)
- `third_party_libraries:` pins CDN library versions with SRI hashes

## Deployment

Push to `main` triggers `.github/workflows/deploy.yml`, which:
1. Builds with `bundle exec jekyll build` (production)
2. Purges unused CSS
3. Deploys `_site/` to GitHub Pages via `JamesIves/github-pages-deploy-action`
