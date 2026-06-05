# Guru Kalyan Jayasingh Website

Personal research website for Guru Kalyan Jayasingh.

## Current Site Structure

The current public template is intentionally small:

- `_layouts/site.html` - full-page shell with theme persistence and page transitions.
- `_layouts/default.html` - general content wrapper.
- `_layouts/archive.html` - list-page wrapper for research, talks, teaching, and blog.
- `_layouts/single.html` - long-form post/publication page wrapper.
- `_layouts/talk.html` - talk detail page wrapper.
- `_includes/site/` - active site chrome:
  - `style.html`
  - `rail.html`
  - `foot.html`
- `_includes/seo.html`, `_includes/base_path`, `_includes/cv-content.html` - active support includes.
- `_pages/` - active top-level routes:
  - Home
  - Projects
  - Research
  - Talks
  - Blog
  - Teaching
  - Academic CV
  - Notes
  - 404
- `_publications/`, `_talks/`, `_teaching/`, `_posts/` - active content collections.
- `images/` - only current public image assets.
- `files/` - public PDFs.

Old academicpages/minimal-mistakes files, demo routes, old mockups, sample images, Sass, JavaScript, and helper tooling are archived under `_legacy/`.

## Local Development

```bash
bundle exec jekyll serve --config _config.yml,_config.dev.yml --host 127.0.0.1 --port 4001
```

Preview:

```text
http://127.0.0.1:4001/
```

Build check:

```bash
bundle exec jekyll build --config _config.yml,_config.dev.yml
```

## Roadmap

See `WEBSITE_ROADMAP.md` for the positioning and improvement backlog.
