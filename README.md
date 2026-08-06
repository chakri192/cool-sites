<div align="center">

<img src="docs/preview.svg" width="840" alt="The page: title, category filters, and a grid of site cards with custom icons" />

# Cool Sites

**A curated directory of unusual and technically interesting websites.**

A single HTML file. No framework, no build step, no analytics, and no network request other than fonts.

<p>
  <img alt="Stack" src="https://img.shields.io/badge/HTML%20·%20CSS%20·%20JS-vanilla-1c1c1e?style=flat-square&logo=html5&logoColor=E34F26" />
  <img alt="Build" src="https://img.shields.io/badge/build%20step-none-1c1c1e?style=flat-square" />
  <img alt="Dependencies" src="https://img.shields.io/badge/dependencies-0-1c1c1e?style=flat-square" />
  <img alt="Host" src="https://img.shields.io/badge/GitHub%20Pages-live-1c1c1e?style=flat-square&logo=githubpages&logoColor=white" />
</p>

**[chakri192.github.io/cool-sites](https://chakri192.github.io/cool-sites/)**

</div>

---

## Contents

Seventeen sites across seven filterable categories.

| Category | Sites |
|---|---|
| Interactive | Neal.fun · Quick Draw! · Akinator |
| Music | Radio Garden · Patatap |
| Explore | GeoGuessr · 100,000 Stars |
| Weird | The Useless Web · Scream Into the Void |
| Creative | This Is Sand |
| Science | This Person Does Not Exist · Loopy |
| Tech | WebGL Fluid Simulation · The Evolution of Trust · Parable of the Polygons · Google Experiments · Shadertoy |

Selecting a category filters the grid with an animated transition, and hovering a card expands its truncated description.

## Implementation

Plain HTML, CSS, and a small amount of vanilla JavaScript in a single file. The only external request is the Google Fonts stylesheet — Plus Jakarta Sans for headings and Nunito for body text.

Each site icon is a hand-authored inline SVG rather than an emoji or icon font. This requires more initial work and in exchange the page carries no icon dependency, renders identically across platforms, and remains sharp at any zoom level.

Filtering is a class toggle over `data-cat` attributes. There is no state management because there is no state: the category buttons set a single attribute and CSS performs the rest.

## Local use

```sh
git clone https://github.com/chakri192/cool-sites.git
cd cool-sites && open index.html
```

The file works directly from the filesystem; no server is required.

## Deployment

**GitHub Pages** — fork the repository, then **Settings → Pages**, source `main` / root.

**Netlify** — drag `index.html` onto [netlify.com](https://netlify.com) under *Add new site → Deploy manually*.

Any static host is suitable.

## Extending it

To add a site, copy any `.site-item` block and update six values: the `href`, name, description, display URL, `data-cat`, and badge class, then replace the inline SVG.

A new category requires three additions: a `.badge-X` style rule, a filter `<button>`, and `data-cat="X"` on the relevant items.

## Project structure

```
cool-sites/
├── index.html       The page — markup, styles, script, and all icons
└── cool-sites.html  An earlier copy of index.html
```

`cool-sites.html` is a near-identical duplicate differing by a single character in the footer. `index.html` is the file served by GitHub Pages and the one to edit; the duplicate can be removed.

## License

MIT for the page itself. Linked sites belong to their respective authors.

## Contributors

| | |
|---|---|
| [chakri192](https://github.com/chakri192) | Author |
| [aider](https://github.com/Aider-AI/aider) | AI pair programmer |
