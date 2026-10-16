# To the Lighthouse

Pixel art game experiments — Lovecraftian coastal scene with parallax layers.

Dark blues, teals, purples. SpriteLab sprites + DALL-E backgrounds composited with CSS.

## Pages

- **intro.html** — Palette, toolkit, game concepts, getting started
- **lighthouse.html** — SpriteLab prompt iteration: eye cloud (4 versions + animation), lighthouse
- **scene.html** — DALL-E background generation, cliff ratios, parallax prep, layer catalog
- **playground.html** — Parallax layer editor: toggle layers, adjust position/scale/velocity, animate

## Stack

- **SpriteLab** — pixel art sprite generation
- **DALL-E gpt-image-1** — background element generation
- **CSS mix-blend-mode: lighten** — layer compositing (black = transparent)
- **Godot 4** — target game engine (future)

## Key learnings

- DALL-E can't enforce spatial constraints — generate elements separately and composite with CSS
- Generate each layer on solid black, use `mix-blend-mode: lighten` to stack
- Match aspect ratios between generated elements and target viewport
- CSS-only base layers (sky gradient, ocean color) guarantee palette consistency
