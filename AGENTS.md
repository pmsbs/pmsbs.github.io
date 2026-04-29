# AGENTS.md

## Project

- **Type**: Jekyll GitHub Pages site (static)
- **Custom domain**: `pmsbs.sp.gov.br` (see `CNAME`)
- **Deployed automatically** via GitHub Pages — no build step or CI pipeline
- **Language**: Portuguese (pt-BR)

## Commands

- **Local dev**: `bundle exec jekyll serve` (requires Bundler + Jekyll)
- **Verify output**: inspect `_site/` after build

## Architecture

- `_posts/` — content pages (posts act as standalone pages, not blog entries)
- `_layouts/default.html` — single layout used by all pages/posts
- `assets/css/main.scss` — SCSS entry point; front matter (`---`) required for Jekyll to process it
- `_sass/` — partial SCSS modules (`_base`, `_container`, `_page`, `_navbar`, `_header`, `_footer`, `_post`)
- `assets/images/` — static images (logo at `assets/images/logo.png`)
- `_config.yml` — site config; `url` and `baseurl` are intentionally empty

## Conventions

- Post filenames: `YYYY-MM-DD-slug.md`
- Posts use `layout: default` and a `title` front matter field
- No JavaScript — pure HTML/CSS
- Primary color: `#095B2E` (defined in `_sass/_base.scss`)
- Font: Roboto via Google Fonts

## Gotchas

- `_site/`, `.jekyll-cache/`, `vendor/` are gitignored — do not commit build artifacts
- SCSS partials must be prefixed with `_` to avoid standalone compilation
- The `main.scss` must have empty front matter (`---\n---`) at the top for Jekyll to process it
- No Gemfile tracked — Jekyll is expected to be installed globally or managed externally
