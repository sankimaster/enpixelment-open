# enpixelment-open — public presets

Small, self-contained pages for individual ENPIXELMENT looks. One folder per project:

```
presets/<name>/
  README.md          what it is, the controls
  preset.json        the values the page starts with
  webgpu/index.html  one file, everything inlined
  webgl/index.html   the same picture for WebGL 2
```

## Read this before you change anything

- 🔴 **The pages are GENERATED.** Do not edit an `index.html` by hand: the next export overwrites it, and a hand edit
  is a copy that no longer matches its source. A change to a page, its look or its code is made at the source and the
  page is exported again. The header comment of each page says it was generated.
- The source of every page lives in a private project, not here. A session that opens only this repo cannot rebuild a
  page; it can read, review and report. To change one, work in the source project (the lab's `public-export` skill is
  the checklist) and export to this folder.
- Each page is one file with its shader, script and styles inline, so it opens by double-click and nothing is fetched.
  Keep it that way: no CDN, no build step, no dependencies.
- A new project is a new folder under `presets/`. Never put a second project's files into an existing one.
- WebGPU is the reference page; the WebGL page is the same shader translated to GLSL and must draw the same picture.
- Do not commit anything that names private projects, local paths or people. Generated pages are scanned for this
  at export; check anything that did not come from an export.

## Licence

Decided by the owner on 2026-10-16: **everything is MIT** (`LICENSE`): code, shaders and preset values alike. A first
version split the preset out under a non-commercial licence; it was dropped the same day, because a restriction on a
few numbers could not be defended and helped nobody. Do not add a second licence or a restriction without being told.
