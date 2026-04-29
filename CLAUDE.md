# Cleave Studios — Project Orientation

This repo is the design-doc and brainstorm monorepo for **Cleave
Studios**, a solo-dev indie JRPG studio prepping a five-game slate.
There is **no code yet** — everything here is markdown.

## Locked decisions (do not relitigate without explicit ask)

- **Team**: solo dev.
- **Engine**: Godot 4.
- **Platforms**: Steam-first; mobile ports later.
- **Monetization**: premium one-time purchase + paid chapter
  expansions. **No gacha, no FOMO, no live-ops.**
- **Art**: pixel art at 32×32 or 48×48, one scale per game. Single
  contracted character artist per game, brought in only after the
  paper prototype validates the loop. See `docs/ART-BIBLE.md`.
- **IP**: original world names, taxonomies, silhouettes. Patent-
  avoidance verbs in place of catch / throw / mount (table below).
  See `docs/IP-GUIDELINES.md`.
- **Localization**: translation table from day one; English at launch.
- **Repo layout**: monorepo subfolders (`games/<name>/`, `shared/`,
  `docs/`). Feature branches live within. Projects can graduate to
  their own repo when they enter full Steam production.
- **Studio name**: Cleave Studios (auto-antonym — *split apart* and
  *cling tightly* — covers all five titles). Prior working name
  *Phoenix Games* is superseded.

A sixth concept, **Wardens of the Veil**, was dropped early — do not
revive without explicit ask.

## The slate

| # | Title | Genre | Verb | Identity |
|---|---|---|---|---|
| 1 | **Ember & Echo** *(default lead)* | FE-style grid tactics | bind | emotions as party characters |
| 2 | **Constellate** | ATB-style 4v4 party JRPG | summon | zodiac flagship; full celestial cosmology |
| 3 | **Chorus** | FE-style grid tactics | compose | positioning *is* the magic system |
| 4 | **Grafted** | party-combat RPG with creature crafting | build / graft | every roster unique; crafting depth |
| 5 | **The Lasting** | ATB-style party RPG, time-loop | remember | knowledge-gating across resets |

Per-game stubs: `games/<name>/README.md`. Full design docs
(`DESIGN.md`, `LORE.md`, `CREATURES.md`, `prototype/`) land in
Phase 1+.

Only **Constellate** uses zodiac mechanically. **The Lasting** uses
zodiac as light narrative flavor. The other three avoid zodiac
entirely.

## Reference taste

JRPG-rooted: Pokémon, Digimon, Fire Emblem, Final Fantasy, Outer
Wilds (knowledge-gating). Reference the *grammar* (tactics grids,
ATB, branched evolution, support conversations) — never the IP.

## Repository layout

```
.
├── CLAUDE.md                        — this file
├── GAMES.md                         — slate index, one line per game
├── README.md                        — minimal placeholder
├── docs/
│   ├── BRAND.md                     — studio identity, voice, namespace
│   ├── IP-GUIDELINES.md             — originality bar, verbs, zodiac rules
│   └── ART-BIBLE.md                 — pixel-art standards, shared pipeline
├── games/
│   ├── ember-and-echo/README.md     — quick spec + pointer to plan
│   ├── constellate/README.md
│   ├── chorus/README.md
│   ├── grafted/README.md
│   └── the-lasting/README.md
├── references/
│   ├── original-plan.md             — 8-batch transcription + synthesis
│   └── original-plan/               — source screenshots
└── shared/README.md                 — populated when Phase 3 begins
```

`references/original-plan.md` is **authoritative** for any detail
not yet in `docs/` or `games/`.

## Where we are

**Phase 0 — Studio setup.** Brand, IP guidelines, art bible, and repo
structure are in place. Next is **Phase 1** — write a one-page
`DESIGN.md` for each of the five games, in parallel. Default starting
order: Ember & Echo first.

The plan is to **prep all five in parallel as design docs and paper
prototypes**, then pick the most-fun-in-five-minutes as the lead and
build a vertical slice. Do not commit to full production on any title
before the paper-prototype phase ends. See
`references/original-plan.md` → "Sequencing strategy" for the full
six-phase plan and verification gates.

## Conventions

**Doc style.**

- One page where possible. Padding hides decisions.
- Short sentences, concrete nouns, no hype adjectives, no exclamation
  marks (this is the studio voice — apply it to internal docs too).
- Tables for anything enumerable (slate, verbs, factions, palettes).
- Cross-link siblings rather than duplicate content.

**Naming new IP** (game, faction, creature, class, region). Before
the name lands in a public-facing doc, run the existence pass from
`docs/IP-GUIDELINES.md`:

1. Steam search (titles + dev/publisher pages).
2. itch.io search.
3. USPTO TESS in classes 9 (downloadable game software) and 41
   (entertainment services).
4. Generic web search.

Document any meaningful collision in the project's `LORE.md` or
`DESIGN.md`.

**Silhouette discipline.** Every creature must read as a unique
silhouette at sprite scale. If two creatures could be confused at
32×32 in monochrome, one must change. Silhouettes must be original —
no derivative shapes from Pokémon, Digimon, MTG, or other
creature-collector franchises.

## Operating notes for assistants

- This repo is documentation-first. Don't add source code, scaffolds,
  or build tooling without explicit ask.
- Don't add per-game `DESIGN.md` / `LORE.md` / `CREATURES.md` files
  pre-emptively — those land in Phase 1+ and should be done
  deliberately, not ahead of schedule.
- When proposing a new IP name, run the naming-collision check above
  before landing it.
- Develop on a feature branch within the monorepo; do not push to
  `main` directly.
- Keep commits scoped (one phase artifact per commit when possible),
  with messages that describe the *decision*, not just the file
  touched.
