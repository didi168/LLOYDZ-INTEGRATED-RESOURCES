# Images

This folder holds the photography used across the site. Every `<img>` in `index.html`
points at a **`.jpg`** here and automatically falls back to the matching **`.svg`**
placeholder if the real photo isn't present yet.

## How to add your real images

1. Save your photo with the **exact filename** from the table below (e.g. `hero.jpg`).
2. Drop it into this `images/` folder.
3. Reload the page — the placeholder is replaced automatically. **No code changes needed.**

> The fallback is wired with `onerror` on each `<img>`, so a missing/renamed file
> simply shows the labelled `.svg` placeholder instead of a broken image.

## Recommended images & sizes

| Filename        | Where it appears            | Recommended size | Orientation | Notes |
|-----------------|-----------------------------|------------------|-------------|-------|
| `hero.jpg`      | Hero, right-hand frame      | 1080 × 1350      | Portrait    | Team on site / flagship asset. Strong, well-lit. |
| `about.jpg`     | About section frame         | 1080 × 1280      | Portrait    | Engineers at work, control room, or site. |
| `project-1.jpg` | Projects — Oil & Gas        | 1000 × 850       | Landscape   | Offshore / process module. |
| `project-2.jpg` | Projects — Energy           | 1000 × 850       | Landscape   | Gas plant / facility. |
| `project-3.jpg` | Projects — Infrastructure   | 1000 × 850       | Landscape   | Highway / bridge. |
| `project-4.jpg` | Projects — Power            | 1000 × 850       | Landscape   | Substation / transmission. |
| `project-5.jpg` | Projects — Asset Integrity  | 1000 × 850       | Landscape   | Tanks / inspection. |
| `project-6.jpg` | Projects — Industrial       | 1000 × 850       | Landscape   | Manufacturing / plant. |

## Tips

- Keep files **under ~300 KB** each — compress with [squoosh.app](https://squoosh.app)
  or `tinyjpg.com`. Large images slow first load.
- Prefer **landscape 1000 × 850** for project tiles and **portrait** for hero/about
  so the framing matches the layout. Photos are cropped with `object-fit: cover`.
- `.webp` works too — if you use it, change the extension in the matching `<img src>`.
- The `.svg` placeholders can stay in the folder; they're tiny and only show when a
  `.jpg` is missing.
