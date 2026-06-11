#  Cool Sites

A curated, hand-picked list of weird, wonderful, and technically impressive corners of the internet — built as a clean, fast, static HTML page with no frameworks, no ads, and no tracking.

**Live site:** https://chakri192.github.io/cool-sites/

---

## What's inside

12 general sites + 5 tech/interactive picks, organized into filterable categories:

| Category | Sites |
|----------|-------|
| Interactive | Neal.fun, Quick Draw!, Akinator |
| Music | Radio Garden, Patatap |
| Explore | GeoGuessr, 100,000 Stars |
| Weird | The Useless Web, Scream Into the Void |
| Creative | This Is Sand |
| Science | This Person Does Not Exist, Loopy |
| Tech | WebGL Fluid Simulation, Evolution of Trust, Parable of the Polygons, Google Experiments, Shadertoy |

---

## Tech stack

- Pure HTML + CSS + vanilla JS — zero dependencies, zero build step
- Custom SVG icons per site (no emojis, no external icon fonts)
- Fonts: [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans) + [Nunito](https://fonts.google.com/specimen/Nunito) via Google Fonts
- Filter by category with animated re-entry
- Hover expands truncated descriptions

---

## Deploy your own

### Option 1 — GitHub Pages (recommended, free)

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Your site is live at `https://YOUR-USERNAME.github.io/REPO-NAME`

### Option 2 — Netlify (drag & drop)

1. Go to [netlify.com](https://netlify.com) → **Add new site → Deploy manually**
2. Drag the `index.html` file onto the deploy area
3. Get a live URL instantly

---

## Customise

**Add a site** — copy any `.site-item` block in `index.html`, update the link, name, description, URL, category (`data-cat`), badge class, and SVG icon.

**Add a category** — add a `.badge-X` style, a filter `<button>`, and use `data-cat="X"` on items.

---

## License

MIT — do whatever you want with it.

### AI tooling

Documentation assisted by local LLMs via [Ollama](https://ollama.com):

| Model | Used for |
|-------|----------|
| `qwen2.5-coder:7b` | Code suggestions, refactoring |
| `llama3.1:8b` | Prose, documentation, commit messages |
