# Matrix Pages

A grid of tiles. Now and then one rises on an edge and turns over, like a page, into a free neighbour.

## Run it

Open `webgpu/index.html` in a recent Chrome or Edge, or `webgl/index.html` in any browser with WebGL 2. Each is one file with everything in it, so a double-click is enough. The two draw the same picture: the WebGL page is the same shader translated to GLSL.

## Controls

**Grid**: Columns, Gap between cells, Corner rounding  
**Motion**: Density (occupied cells), Flip rate (per tile / s), Speed  
**Colour**: Base hue, Colour range, Shadow  
Buttons: Pause, New seed (a different history), Save PNG.

`preset.json` holds the values the page starts with.

## Licence

MIT (`../../LICENSE`), for everything here: the code, the shaders and the preset values. Use it, change it, ship it;
keep the copyright notice. A credit such as *"Matrix Pages by ENPIXELMENT"* is appreciated.
