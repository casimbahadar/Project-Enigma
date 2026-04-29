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

## Solo-art realities

The studio's working assumption is **zero art-commission budget**
through Phase 4. Pixel art at 32×32 / 48×48 was chosen specifically
because a determined solo dev can produce it. The contracted artist
in the production model above is an *optional upgrade* if budget
exists at Phase 5, not a requirement.

### Tooling stack (free or near-free)

| Need | Tool | Cost |
|---|---|---|
| Pixel art editor | Aseprite | $20 one-time |
| Free alternative | LibreSprite (Aseprite fork) | Free |
| Lightweight web editor | Piskel | Free |
| Tilemap design | Tiled | Free |
| Audio editing | Audacity | Free |
| Music composition | LMMS | Free |

Aseprite + Tiled + Audacity is the production stack used by most
solo-dev pixel-art Steam releases. No additional tooling is
required to ship.

### Asset-pack policy

Free / CC0 asset packs are **acceptable for shipped releases** under
the following rules:

- **Permitted**: Kenney.nl (CC0), OpenGameArt.org assets explicitly
  marked CC0 or compatible, itch.io free asset bundles where the
  license allows commercial use.
- **Required**: read every license before use. Some "free" packs
  require attribution; some prohibit commercial use; some require
  share-alike terms that conflict with the studio's premium model.
- **Preferred over packs**: assets *modified* by the solo dev to
  match the game's locked palette and silhouette discipline. A
  Kenney sprite re-palettized into Ember & Echo's color scheme reads
  as the game's, not as a pack.
- **Avoid**: visibly-Kenney UI elements (fonts, buttons) without
  recolor. Players recognize stock Kenney UI; using it raw signals
  "asset-flip" even when the rest of the game is original.

### When commissioning is justified

Three places where commissioning has measurably higher marketing
return than DIY, in priority order if budget exists:

1. **Steam capsule art** ($200–$500). The single most important
   marketing asset on Steam. If any single piece of art gets
   commissioned, this is it.
2. **Music / SFX** ($300–$1,500 for 5–10 tracks). Pixel art
   communicates fine when self-produced; bad audio reads as cheap.
   Higher per-dollar return than additional art commissioning.
3. **Trailer key art / one or two illustrations for marketing**
   ($200–$800). Only after capsule + audio are handled.

Character sprites, tilesets, UI, and creature rosters are **last
priority for commissioning**. They benefit most from the studio's
own visual identity and least from outside polish.

### Per-game art burden — sequencing implication

Ranked from lightest to heaviest art burden for a solo dev:

| Rank | Game | Notes |
|---|---|---|
| 1 | The Lasting | No creature roster. 12 companion portraits + kingdom NPCs + a few region tilesets. Highest reuse across loops. |
| 2 | Ember & Echo | ~50 unique Echoes across the full game; V-slice needs 4 + 1 evolution. Moderate, manageable solo. |
| 3 | Chorus | 12–20 characters + distinct musical-genre region tilesets per chapter. No creature roster. Moderate. |
| 4 | Grafted | Procedural-sprite system means *parts*, not whole creatures. Each part must compose with every other part — art-engineering burden is real, but total unique sprites is smaller. |
| 5 | Constellate | 36+ named creatures across 12 constellations. Heaviest by design — that's why it's the capstone. |

This burden ranking is one of the reasons the locked release order
(see `docs/RELEASE-STRATEGY.md`) places Constellate last. By the
time the studio reaches its art-heaviest title, four prior releases
have generated revenue and Grafted's procedural-sprite system is
already in `shared/`, dramatically reducing Constellate's per-
creature cost.

### Practical solo-dev habits

- **Develop a baseline before Phase 3.** Spend an evening or two
  with Aseprite tutorials before the V-slice begins. Solo-dev
  pixel art is a respected aesthetic in the indie scene; rough
  sprites that look like *yours* beat polished sprites that look
  generic.
- **Reuse aggressively.** The `shared/` pipeline (palette discipline,
  animation conventions, sprite import settings) exists so per-title
  art burden compounds *down* across the slate, not up.
- **Don't commission before Phase 4.** Placeholder art is fine for
  paper prototypes and the V-slice. Save money for the moment
  commissioning has measurable marketing return.
- **AI tools for concepting only.** Stable Diffusion / Midjourney
  are acceptable for *brainstorming* silhouettes and palettes that
  the dev then redraws as pixel art. AI output is not shipped
  directly — both for IP-cleanliness reasons and because it reads
  as inconsistent against hand-drawn pixel work.
