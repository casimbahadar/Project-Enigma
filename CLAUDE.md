# Cleave Studios — Project Orientation

This repo is the design-doc and brainstorm monorepo for **Cleave
Studios**, a solo-dev indie JRPG studio prepping a five-game slate.

## Locked decisions (do not relitigate without explicit ask)

- **Team**: solo dev.
- **Engine**: Godot 4.
- **Platforms**: Steam-first; mobile ports later.
- **Monetization**: premium one-time purchase + paid chapter
  expansions. **No gacha, no FOMO, no live-ops.**
- **Art**: pixel art at 32×32 or 48×48. Single contracted character
  artist per game, brought in only after the paper prototype validates
  the loop. See `docs/ART-BIBLE.md`.
- **IP**: original world names, taxonomies, silhouettes. Patent-
  avoidance verbs in place of catch / throw / mount: **bind, summon,
  compose, build/graft, remember**. See `docs/IP-GUIDELINES.md`.
- **Localization**: translation table from day one; English at launch.
- **Repo layout**: monorepo subfolders (`games/<name>/`, `shared/`,
  `docs/`). Feature branches live within. Projects can graduate to
  their own repo when they enter full Steam production.

## The slate

Five titles, in default release order:

1. **Ember & Echo — Memory-Bound Tactics** *(lead)*
2. **Constellate — Star-Forged Companions** *(zodiac flagship)*
3. **Chorus — Music-Powered Tactical RPG**
4. **Grafted — Build-A-Beast Bio-punk RPG**
5. **The Lasting — Time-Loop JRPG**

Per-game stubs: `games/<name>/README.md`. Full design docs (`DESIGN.md`,
`LORE.md`, `CREATURES.md`, `prototype/`) land in Phase 1+.

A sixth concept, **Wardens of the Veil**, was dropped early — do not
revive without explicit ask.

## Reference taste

JRPG-rooted: Pokémon, Digimon, Fire Emblem, Final Fantasy. Reference
the *grammar* (tactics grids, ATB, branched evolution, support
conversations) — never the IP.

## Where to look

- `docs/BRAND.md` — studio identity, voice, namespace status,
  hygiene checklist.
- `docs/IP-GUIDELINES.md` — originality bar, patent-avoidance verbs,
  zodiac handling rules.
- `docs/ART-BIBLE.md` — pixel-art standards and shared pipeline.
- `docs/RELEASE-STRATEGY.md` — slate sequencing, per-title platform
  fit, mobile monetization, revenue checkpoints.
- `GAMES.md` — slate index (one-line per game).
- `games/<name>/README.md` — per-game quick spec + pointer to plan.
- `games/<name>/DESIGN.md` — one-page design brief (hook, loop, IP,
  episodic plan, V-slice scope).
- `games/<name>/prototype/PROTOTYPE.md` — paper-prototype brief for
  Phase 2 testing.
- `references/original-plan.md` — full transcription of the original
  brainstorm session, in 8 batches with synthesis. Authoritative for
  any detail not yet in `docs/` or `games/`.

## Where we are

- ✅ **Phase 0 — Studio setup.** Brand, IP guidelines, art bible,
  release strategy, and repo structure are in place.
- ✅ **Phase 1 — Design docs in parallel.** All five `DESIGN.md`
  one-pagers are landed.
- 🟡 **Phase 2 — Paper prototypes (in progress).** All five
  `PROTOTYPE.md` briefs are staged. Next gate is the physical
  kitchen-table test sessions; the goal is to identify the project
  whose core loop is most fun in 5 minutes.
- ⬜ Phase 3 — pick lead, build vertical slice
- ⬜ Phase 4 — validate (itch.io demo + Steam Next Fest, 5,000
  wishlist target)
- ⬜ Phase 5 — full production of lead title
- ⬜ Phase 6 — studio compounding

## Slate release order (per `docs/RELEASE-STRATEGY.md`)

`Ember & Echo → Grafted → The Lasting → Chorus → Constellate.`
Sequencing accounts for engine reuse, mobile-platform fit, and
capstone toolkit assembly (Grafted's procedural-sprite system feeds
Constellate's 36+ creature roster).

## Sequencing reminder

The plan is to **prep all five in parallel as design docs and paper
prototypes**, then pick the most-fun-in-five-minutes as the lead and
build a vertical slice. Do not commit to full production on any title
before the paper-prototype phase ends. See
`references/original-plan.md` → "Sequencing strategy" for the full
six-phase plan and verification gates.

## Operating notes for assistants

- This repo is documentation-first; there is no code yet. Don't add
  source code, scaffolds, or build tooling without explicit ask.
- Keep new docs concise — one page where possible. Padding hides
  decisions.
- When proposing a new IP name (game, faction, creature, class), run
  the naming-collision check from `docs/IP-GUIDELINES.md` before
  landing it.
