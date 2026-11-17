# Mainloop brand assets

The visual identity for Mainloop, "Amber Terminal": an open-loop glyph in warm amber on ink, with a monospace wordmark. The glyph is a process that has not finished. The palette is borrowed from CRT terminals.

The loop opens downward: the 90 degree gap sits at 6 o'clock. A blinking cursor appears in the wordmark only, never in the glyph.

Tagline: `// still running_`

## Palette

| Token | Hex | Use |
|---|---|---|
| ink | `#101014` | primary ground, glyph on amber |
| panel | `#17181D` | raised surfaces |
| amber | `#F2A33C` | the accent: glyph on ink, links, cursor |
| bone | `#E8E3D8` | text on ink |
| mute | `#6B6E78` | secondary text |

Take colors from this table instead of sampling a PNG.

## Type

- Wordmark: Cascadia Code SemiBold, lowercase. `main` is bone, `loop` is amber, with a blinking `_` cursor where animation is possible. Fallbacks: Consolas, ui-monospace.
- Body: Segoe UI or the system sans. The monospace is the brand voice, not the reading face.

## Assets

All files are in `assets/`, 512 by 512 PNG.

| File | Purpose |
|---|---|
| `play-store-icon-512.png` | Google Play app icon: full-bleed amber, ink glyph |
| `github-avatar-512.png` | GitHub organization avatar: ink tile, amber glyph |
| `adaptive-foreground-512.png` | Android adaptive-icon foreground: transparent, glyph inside the 66% safe zone; pair with a solid `#F2A33C` background layer |
| `monochrome-512.png` | Android 13+ themed-icon layer: white glyph on transparent |

## Glyph geometry

The glyph is drawn in a 96-unit viewBox: an arc of radius 30, stroke width 8, sweeping 270 degrees, with the gap at 6 o'clock. There is no cursor block. The PNGs were rendered at 4x supersampling.

As inline SVG:

```svg
<path d="M 69.21 26.79 A 30 30 0 1 1 26.79 26.79" transform="rotate(180 48 48)" fill="none" stroke="#F2A33C" stroke-width="8" stroke-linecap="round"/>
```

## Usage

Anything rendering the glyph uses the 6 o'clock gap and the wordmark-only cursor. Use the assets as they are; do not recolor outside the palette.

## License

All rights reserved.
