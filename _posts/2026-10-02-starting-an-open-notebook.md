---
title: "Starting an open notebook"
date: 2026-10-02 10:00:00 -0700
project: Notebook setup
status: complete
tags: [meta, open-science]
---

Today I set up this open lab notebook with Jekyll and GitHub Pages, so my day-to-day research notes are public and version-controlled.

## Goal

Have a place to publish dated research entries — methods, results, and dead ends — with almost no friction.

## Methods

- Jekyll site hosted on GitHub Pages from the `main` branch.
- One Markdown file per entry in `_posts/`, named `YYYY-MM-DD-title.md`.
- Front matter fields: `project`, `status`, `tags`.
- A blank entry template lives in `_templates/entry-template.md`.

## Results

Entries render with dates, project and tag links, math support (e.g. $E = mc^2$), and a link to each entry's edit history on GitHub.

| Feature            | Where                  |
|--------------------|------------------------|
| Entries by month   | Home page              |
| Grouped by project | `/projects/`           |
| Grouped by tag     | `/tags/`               |
| Feed               | `/feed.xml`            |

## Next steps

- [ ] Write the first real research entry
- [ ] Fill in the About page with contact details
