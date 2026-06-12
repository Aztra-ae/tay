# IsoEngine 🎮

A browser-based isometric game engine with a tilted map, character control, NPC, and a drag-and-drop level editor — all in one `index.html` file.

## Play it live

> **GitHub Pages URL:** `https://<your-username>.github.io/<your-repo-name>/`

---

## Features

| Feature | Details |
|---|---|
| **Isometric Map** | 16×16 tilted grid with 8 tile types |
| **Edit Mode** | Click/drag to paint tiles |
| **Drag & Drop Mode** | Drag tiles from palette onto the map |
| **Play Mode** | WASD / arrow keys to move your character |
| **NPC** | Walk near the wizard to trigger dialogue |
| **Camera** | Scroll to zoom, middle-drag to pan, R to reset |
| **Animated Tiles** | Water ripples, lava pulses |
| **Level Generator** | One-click procedural terrain |

## Controls

| Action | Input |
|---|---|
| Move | W A S D or arrow keys |
| Sprint | Hold Shift |
| Zoom | Mouse wheel |
| Pan camera | Middle-click drag |
| Reset camera | R |

## How to host on GitHub Pages

1. Create a new GitHub repository (public)
2. Drop index.html into the root
3. Go to Settings → Pages
4. Set source to main branch, / (root) folder
5. Click Save — your game will be live in ~60 seconds

That's it. No build step, no dependencies, no server needed.

## Project structure

```
/
└── index.html   ← the entire game (HTML + CSS + JS)
└── README.md
```

## Extending the engine

- Add tiles: extend the TILES array at the top of the script
- Larger maps: change COLS and ROWS constants
- More NPCs: duplicate the npc object and add to the render loop
- Save/load levels: JSON.stringify(map) → localStorage
