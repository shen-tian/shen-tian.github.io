# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal tech blog (shentian.me) built with Jekyll 4 and the Minima 2 theme, hosted on GitHub Pages.

## Development Setup

Requires Ruby (version in `.ruby-version`) via rbenv:

```bash
brew install rbenv          # if needed
rbenv install $(cat .ruby-version)
bundle install
```

## Development Commands

```bash
# Serve locally at localhost:4000
bundle exec jekyll serve

# Build without serving
bundle exec jekyll build
```

Note: `_config.yml` changes require restarting `jekyll serve`.

## Architecture

- **`_posts/`** — Published blog posts (named `YYYY-MM-DD-title.md` with YAML front matter)
- **`_drafts/`** — Unpublished drafts (same format, no date prefix needed)
- **`_includes/google-analytics.html`** — Custom GA4 include (overrides Minima's default; only injected in production)
- **`_config.yml`** — Site metadata and `google_analytics` tracking ID (GA4: `G-PPC6306M88`)
- **Theme** — Uses the `minima` gem theme; layouts/includes come from the gem unless overridden in `_includes/` or `_layouts/`
- **Markdown** — Kramdown with GFM parser (`kramdown-parser-gfm`)
