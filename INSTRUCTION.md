# INSTRUCTION — How to modify layout, templates, and content

> Quick reference for editing this Academic Pages / Minimal Mistakes Jekyll site. Use these notes to find which files control layout, content, styles, and how to preview changes locally. ✅

---

## 1) Quick map — where things live 🔍

- **Site configuration**: `_config.yml` — site title, author info, theme, feeds, collections.
- **Navigation**: `_data/navigation.yml` — order and links in the header.
- **Header / Masthead**: `_includes/masthead.html` — markup for top menu and title.
- **Layouts (page wrappers)**: `_layouts/` — e.g. `default.html`, `single.html`, `archive.html`, `talk.html`.
- **Reusable partials**: `_includes/` — `footer.html`, `head.html`, `author-profile.html`, `page__hero.html`, etc.
- **Content (Markdown)**:
  - Pages: `_pages/*.md` (e.g., `about.md`)
  - Posts: `_posts/YYYY-MM-DD-slug.md`
  - Collections: `_talks/`, `_publications/`, `_teaching/`, `_portfolio/` (one Markdown file per item)
- **Data & labels**: `_data/*.yml` — `navigation.yml`, `ui-text.yml`, `authors.yml`.
- **Styling**: `_sass/` and `assets/css/main.scss` — themes and variables (`_sass/theme/_*.scss`, `_sass/layout/_*.scss`).
- **JS behavior**: `assets/js/` — theme JS, toggles, nav behavior.
- **Generated output**: `_site/` — built site (do NOT edit this directly).

---

## 2) Common edits — exact files & examples ✏️

### Change site title, description, or author
Edit: `/_config.yml`

Example change:

```yaml
# before
title: "Your Name / Site Title"

# replace with
title: "Jack Yang — Sun Chaser"
```

> After changing `_config.yml` restart the dev server.

### Add / reorder header links
Edit: `/_data/navigation.yml`

Add an item:

```yaml
main:
  - title: "Projects"
    url: /portfolio/
```

This updates the masthead menu (the markup is generated from `site.data.navigation.main`).

### Change masthead markup or add controls
Edit: `/_includes/masthead.html`

You can change structure, add classes, or insert a new element (a site badge, search input, etc.).

### Modify the page around content (header/footer placement)
Edit: `/_layouts/default.html`

This file includes the masthead and footer includes and contains `{{ content }}` where page bodies are inserted.

### Edit the author box shown on sidebars
Edit: `/_includes/author-profile.html` and `_config.yml` -> `author:` fields or `_data/authors.yml`.

### Change footer text
Edit: `/_includes/footer.html` and/or `/_includes/footer/custom.html` (if present)

### Edit a page's content
Edit: `/_pages/about.md` or other page files. Change front matter or Markdown body.

Front matter example (top of a page file):

```yaml
---
title: "My Talk"
author_profile: true
permalink: /talks/my-talk/
---
```

### Create or edit posts
- Add a file to `_posts/` with name `YYYY-MM-DD-your-post-title.md` and add front matter `title:` `date:` `categories:` etc.

### Modify colors and theme variables
Edit: `_sass/theme/_default_light.scss` (or whichever `_theme` you use)

Change variables like `$masthead-height` or color tokens such as `$footer` to update site-wide visuals.

---

## 3) Preview changes locally ▶️

Start dev server (recommended):

```bash
bundle _2.5.6_ exec jekyll serve -l -H localhost
```

Notes:
- If you change `_config.yml` stop and restart the server (it is not hot-reloaded).
- The site will be built to `_site/`; open `http://localhost:4000` to preview.

---

## 4) Tips & gotchas 💡

- Edit source files (not `_site/`) — the latter is auto-generated.
- Use includes and layouts for structural changes to avoid touching many files.
- Theme variables in `_sass/theme` allow quick color/spacing changes across the whole site.
- For content driven by data (menus, labels), prefer editing `_data/*.yml` rather than templates.
- Always commit changes in a branch and preview before pushing to GitHub pages.

> Quick checklist:
> - Update `_config.yml` for global settings
> - Edit `_data/navigation.yml` to change header links
> - Edit includes (`_includes/*`) for small reusable components
> - Edit `_layouts/*` for structural/template changes
> - Edit `_sass/*` for styling
> - Restart `jekyll serve` if you change `_config.yml`

---

If you'd like, I can make one small example edit (e.g., change `title` in `_config.yml` and add a "Projects" link to `navigation.yml`) and show the patch. 🔧

---

(More help: open any filename and I will point to the exact line to edit.)
