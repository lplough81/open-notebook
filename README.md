# Open Notebook

An open lab notebook built with [Jekyll](https://jekyllrb.com) and hosted on GitHub Pages at
**https://lplough81.github.io/open-notebook/**

## Turn on GitHub Pages (one time)

1. On GitHub go to **Settings → Pages**.
2. Under *Build and deployment*, choose **Source: Deploy from a branch**, **Branch: `main` / `(root)`**, and save.
3. After a minute or two the site is live at the URL above.

## Add a notebook entry

1. Copy `_templates/entry-template.md` into `_posts/` and rename it `YYYY-MM-DD-short-title.md`.
2. Fill in the front matter (`title`, `date`, `project`, `status`, `tags`) and write the entry in Markdown.
3. Commit and push — or do it right in the browser with GitHub's **Add file → Create new file**.

Front-matter fields:

| Field     | Purpose                                                     |
|-----------|-------------------------------------------------------------|
| `project` | Groups entries on the **Projects** page                     |
| `status`  | `in progress`, `complete`, `failed`, `on hold` (colour-coded) |
| `tags`    | List, e.g. `[pcr, qc]` — groups entries on the **Tags** page |

Math works with `$inline$` and `$$display$$` (MathJax). Put figures and data files in `assets/data/`
and link them with `{{ '/assets/data/file.png' | relative_url }}`.

## Preview locally (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000/open-notebook/
```

## Layout

```
_config.yml            site settings (title, author, URLs, license)
_posts/                notebook entries, one file per entry
_templates/            blank entry template (not published)
_layouts/              page templates
assets/css/style.css   styling (light + dark mode)
assets/data/           figures, data, scripts
index.html             entry list, grouped by month
projects.html, tags.html, about.md
```
