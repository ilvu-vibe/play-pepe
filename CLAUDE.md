# Play Pepe - Project Guide

## Project Overview
A Mario-style browser game called "Play Pepe" built as a single HTML file using vanilla JavaScript and HTML5 Canvas.

## Game Concept
A footballer (Pepe) runs through a football pitch environment:
- **Jump** to avoid incoming slide tackles from opponents
- **Head** incoming footballs (jump + timing)
- **Slide** to tackle opponents who have the ball

## Tech Stack
- Single `index.html` file
- Vanilla JavaScript (no frameworks/libraries)
- HTML5 Canvas for rendering
- No build tools or dependencies

## File Structure
```
index.html   — entire game (HTML + CSS + JS in one file)
```

## Game Mechanics
- Side-scrolling platformer style (like Mario)
- Player runs forward automatically; player controls: jump and slide
- Obstacles: opponents sliding in, footballs flying in
- Scoring: head a ball = points, slide an opponent = points, survival time = points
- Lives system: getting hit by slide or ball = lose a life

## Controls
- **Space / Up Arrow** — Jump
- **Down Arrow / S** — Slide
- Mouse click also triggers jump (mobile friendly)

## Code Conventions
- All game logic in a single `<script>` tag
- Use `requestAnimationFrame` game loop
- Canvas 2D context for all rendering
- Sprite-style drawing with plain shapes/colors (no image assets required)
- Constants defined at top of script for easy tuning (speeds, sizes, gravity, etc.)

## Art Style
- Pixel-art inspired, drawn with canvas primitives (rectangles, arcs, lines)
- Green pitch background with white line markings
- Pepe character: distinctive appearance (bald head, wide eyes)
- Opponents in red/yellow kits
- Footballs as white circles with black pentagon pattern

## Development Notes
- Keep everything in `index.html` — do not split into multiple files
- No external assets (images, sounds from files) — use canvas drawing only
- Web Audio API allowed for simple sound effects (generated programmatically)
