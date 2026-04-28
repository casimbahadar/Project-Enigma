# Cleave Studios — Art Bible

## Default art form

**Pixel art.** Across the entire slate, for the full duration of the
solo-dev portfolio phase. Pixel art is the format that lets one
person ship five games' worth of visual identity at quality.

## Sprite scale

- **Character / creature sprites: 32×32** as the baseline. Use
  **48×48** when a game's combat camera or readability demands it
  (e.g., creatures with complex silhouettes in *Grafted*).
- **One scale per game.** Don't mix 32 and 48 inside a single project;
  the engine, palette, and animation pipeline are tuned per game.
- **Tilesets**: 16×16 or 32×32 to match the sprite scale.

## Production model

- The solo dev (founder) handles all programmer art, UI, tilesets,
  and prototype creatures.
- A **single contracted character artist per project** is brought in
  **only after the paper prototype validates the loop** (i.e., end of
  Phase 2 / start of Phase 3 in the sequencing plan).
- This is one artist per game, not one studio-wide artist — each
  game gets its own visual identity.

## Cross-project shared pipeline

Anything reusable lives in `shared/` so future projects compound on
prior work:

- **Palette discipline**: each game has a locked palette of ≤32
  colors, designed for readability at sprite scale and for high
  contrast against tilesets.
- **Sprite import settings**: nearest-neighbor filtering, no
  compression, fixed pixels-per-unit.
- **Animation conventions**: idle / walk / hit / attack / death
  frame counts standardized so behavior trees and combat hooks port
  cleanly between games.
- **Pixel-perfect camera setup** in Godot 4 (locked engine; see
  `BRAND.md`).

## Silhouette discipline

- Every creature must be readable as a unique silhouette at sprite
  scale. If two creatures could be confused at 32×32 in monochrome,
  one must change.
- Creature silhouettes must be **original** — no derivative shapes
  from Pokémon, Digimon, MTG, or other creature-collector
  franchises (see `IP-GUIDELINES.md` for the originality bar).
- Each game has one or two **silhouette signatures** that mark its
  visual world (e.g., Constellate's Asterix carry visible starlight
  rings; Grafted's beasts have visible seam-lines where parts join).

## Per-game visual identities (TBD)

When each game's `DESIGN.md` lands in Phase 1, append a per-project
visual brief here covering:

- Palette family (warm / cool / desaturated / high-key etc.)
- Lighting model (flat, dithered, ambient)
- One signature visual element that makes the game instantly
  recognizable.
