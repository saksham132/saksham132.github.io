# Saksham Gupta – personal website

Live at https://saksham132.github.io. Built with Jekyll and served by GitHub Pages (no theme, no plugins).

## Weekly posting

Copy a file from `_templates/` into the matching folder, edit it, then commit and push:

| What | Folder | Template |
| --- | --- | --- |
| Paper summary | `_papers/` | `_templates/paper.md` |
| Guitar video (YouTube link) | `_songs/` | `_templates/song.md` |
| Photo of the week | `_photos/` (image in `assets/photos/`) | `_templates/photo.md` |

The home page, Research page and Off the Bench page update on their own.

## Editing pages

- `index.md` (About me), `research.md`, `off-the-bench.md`
- Nav labels and links in `_config.yml`
- Colors and fonts in `assets/css/style.css`
- CV: replace `assets/GuptaSaksham_CV_GS.pdf` (keep the same filename so the link keeps working)

## Preview locally (optional)

    bundle exec jekyll serve
