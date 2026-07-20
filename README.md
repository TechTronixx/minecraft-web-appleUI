# Minecraft Apple-Style Landing Page

![HTML5](https://img.shields.io/badge/HTML5-markup-e34f26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-vanilla-1572b6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-f7df1e?logo=javascript&logoColor=black)
![License](https://img.shields.io/github/license/TechTronixx/minecraft-web-appleUI)
![Issues](https://img.shields.io/github/issues/TechTronixx/minecraft-web-appleUI)
![Last commit](https://img.shields.io/github/last-commit/TechTronixx/minecraft-web-appleUI)

A single-file, Apple-inspired landing page for Minecraft: Java Edition, built with plain HTML, CSS, and JavaScript — no frameworks, no build step, no dependencies. The whole page lives in `index.html`: markup, styles, and script inline, with draggable 3D CSS cubes, a detonatable TNT block, and two scroll-snap carousels, all styled after Apple's product-page aesthetic.

## Features

- **Apple-style layout** — sticky translucent nav with backdrop blur, a promo ribbon, three full-width hero tiles, a six-card promo grid, two carousels, a closer, and a multi-column footer with footnotes and a legal bar.
- **Interactive 3D blocks** — pixel-textured CSS cubes you can drag to rotate: a grass block, a redstone lamp you tap to toggle its glow, and a TNT block you tap to detonate (fuse flash, particle burst, respawn).
- **Two carousels** — a nine-card biome gallery (Overworld, Nether, End, Deep Dark, Cherry Grove, and more) and a masonry "ways to play" row, both with arrow buttons and dot pagination.
- **Responsive** — single-column grid, collapsed nav, and reflowed carousels down to mobile (<=734px).
- **Accessible** — keyboard-focusable controls, ARIA labels on cubes and carousels, and full `prefers-reduced-motion` support (bob and reveal animations off, smooth scroll becomes instant, TNT detonation becomes a quiet fade).

## Demo

https://github.com/user-attachments/assets/7ac22862-264f-4175-98e6-2ed0c102287c

## Quick start

Open `index.html` in any modern browser. No server or build step required.

```sh
# macOS
open index.html
# Windows
start index.html
# Linux
xdg-open index.html
```

## Requirements

- A modern browser: Chrome, Safari, Firefox, or Edge.
- Optional: an internet connection for the Minecraft pixel font, loaded from `db.onlinewebfonts.com`. If it is blocked or you are offline, the font falls back to Courier New and everything else still works.

## Install (manual)

```sh
git clone https://github.com/TechTronixx/minecraft-web-appleUI.git
cd minecraft-web-appleUI
# then open index.html — see Quick start
```

## Project structure

```
minecraft-web-appleUI/
├── index.html   # entire page — markup, styles, and script inline
└── README.md
```

## Usage

Open the page and browse. The interactions are the point of the demo:

- **Drag** any 3D cube (grass, lamp, TNT, or the blocks in the Mods/Skins cards) to rotate it.
- **Tap** the redstone lamp to toggle its light on and off.
- **Tap** the TNT block to detonate it.
- Use the **arrow buttons or dots** under each carousel to scroll.

## Notes

- Everything is in one file — no external CSS, JS, or image assets. The cubes, biome cards, and icons are drawn with CSS gradients and inline SVG pixel art.
- The only network request is the optional pixel font (see Requirements); block it and the page still renders.
- `prefers-reduced-motion` is respected throughout (see Features).

## Development

There is no test suite. To self-check a change, open `index.html` and verify:

- The nav, ribbon, three hero tiles, six-card grid, two carousels, and footer render.
- Drag a cube to rotate it; tap the lamp to toggle; tap TNT to detonate.
- Resize to <=734px: single-column grid, collapsed nav, reflowed carousels.
- Toggle `prefers-reduced-motion`: bob and reveal animations off, TNT detonation is a quiet fade.

## Contributing

Contributions are welcome. Branch off `main`, keep everything in `index.html`, run the self-checks above, and open a pull request against `main`. Report bugs or request features via [Issues](https://github.com/TechTronixx/minecraft-web-appleUI/issues).

## Disclaimer

This is a fan-made concept page created for learning purposes. It is not affiliated with, endorsed by, or connected to Mojang Studios, Microsoft, or Apple Inc. Minecraft and Minecraft: Java Edition are trademarks of Mojang Studios and Microsoft. The Apple product-page design language is referenced for educational purposes only. No ownership is claimed over any trademarked property.

## License

Licensed under the MIT License. See [LICENSE](LICENSE).
