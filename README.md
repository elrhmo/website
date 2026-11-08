# Elliot Moses — personal website

Source for [elliotmoses.dev](https://elliotmoses.dev), hosted on Cloudflare Workers (config in `wrangler.jsonc`).

Plain HTML and one stylesheet (`style.css`). No build step or dependencies.

## Run locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Layout

Each project lives in its own folder, with its page, thumbnail and images together:

```
projects/bus-departure-board/
  index.html
  thumb.jpg      160×160, shown in the home page list
  board.jpg      images used on the page
```

`images/` holds only site-wide images (the avatar, and the thumbnail for the externally hosted storymap).

## Add a project

1. Copy an existing folder in `projects/` (e.g. `projects/sourdough-calculator/`) to `projects/<new-name>/`.
2. Edit its `index.html`, and replace `thumb.jpg` and any images (keep images around 1200px wide).
3. Add an entry to the project list in `index.html` (newest first).
