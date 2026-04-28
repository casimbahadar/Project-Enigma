# Original Plan — Reconstructed Notes

Notes transcribed from screenshots of the prior brainstorm session
(saved in `references/original-plan/`). Appended per batch as
screenshots come in.

---

## Batch 1 — Direction lock and portfolio framing

### Locked direction

- **Solo dev.** One-person team.
- **Platform:** Steam-first; mobile ports later.
- **Monetization:** premium one-time purchase + paid chapter / expansion DLC.
- **Starting game:** Ember & Echo (subject to paper-prototyping confirmation).

### Portfolio shape

- Five concepts kept on the slate:
  1. Ember & Echo
  2. Constellate
  3. Chorus
  4. Grafted
  5. The Lasting
- A sixth concept, **Wardens**, was dropped. (Detail TBD from later batches.)
- **Zodiacs:** flagship treatment in **Constellate**; light flavor in **The Lasting**; not used in the others.

### Code layout

- Monorepo with subfolders per game.

### Release order

- Lead game to be chosen **after paper prototyping**. Not pre-locked.

### Studio name

- Working name in the original session: **Phoenix Games**.
- Superseded in the current session by **Cleave Studios** (see `STUDIO-NAME.md`).

### Reconciliation with current-session slate read

| Item | Current-session proposal | Original plan | Action |
|---|---|---|---|
| First game | Grafted (mobile, fastest revenue) | Ember & Echo | Defer to original plan |
| Platform per game | Mixed (mobile-first for Grafted) | Steam-first across the board | Defer to original plan |
| Monetization | Implicit per game | Premium + paid DLC chapters | Defer to original plan |
| Release order | Small → flagship | TBD post-prototyping | Don't lock yet |
| Zodiac scope | Three games | Constellate primary, Lasting flavor only | Defer to original plan |
| Team | Implicit | Solo dev | Solo-dev scope discipline applies |

---

## Batch 2 — Overall summary for studio direction

Source file in original session: `1-want-to-develop-effervescent-mind.md`
(working title in the prior session's plan).

### Document title

`Game Studio Portfolio — Multi-Project Plan`

### Context section (transcribed)

- Founding a **solo game studio**.
- Goal: prep **multiple original-IP games** for release over time.
- After exploring **six concept directions**, **five** were selected to develop
  (the dropped one is *Wardens*, per Batch 1).
- Repository state at time of plan: empty, with a stub `README` on the
  working branch.

### Repo structure — locked: monorepo subfolders

- All five projects live in one repository.
- Each game gets its own subfolder under `games/<name>/`.
- Cross-cutting / shared code intended (specifics truncated in screenshot —
  flag for follow-up batches).

### Implications for current branch

- Our current branch (`claude/game-concept-brainstorm-qmzvj`) has so far
  used flat root-level docs (`STUDIO-NAME.md`, `GAMES.md`,
  `references/`). The original plan calls for `games/<name>/` subfolders.
- When we start expanding individual game concepts, switch to
  `games/ember-and-echo/`, `games/constellate/`, etc. so we match the
  locked layout from the original plan.

---

## Batch 3 — Full transcription of Context + Repo-structure prose

Reconstructed by stitching scroll-fragment screenshots of the original
plan document.

### Context (full prose)

> You're founding a solo game studio and want to prep **multiple
> original-IP JRPG concepts in parallel** so the studio can ship a
> series over time. **Steam-first, mobile-port-later, premium
> one-time-purchase** model. Your taste is JRPG-rooted (Pokémon,
> Digimon, Fire Emblem, Final Fantasy), and you specifically want to
> weave **zodiacs** (Western constellations, Western birth signs, and
> Chinese zodiac) into one or more games.
>
> After exploring six concept directions, you've selected five to
> develop in parallel as **design briefs** (dropping **Wardens of the
> Veil**): **Ember & Echo, Constellate, Chorus, Grafted, The Lasting**.
>
> The repository is currently empty (stub README on the working
> branch). This plan defines:
> 1. How to structure the repo for multiple projects.
> 2. A one-page brief per project.
> 3. How zodiacs slot in.
> 4. A realistic sequencing strategy — because a solo dev can *prep*
>    five but can only fully *build* one at a time.

### Repo structure — locked: monorepo subfolders (full prose)

> All five projects live in one repo with `games/<name>/` subfolders.
> Cross-project tooling (save format, dialogue parser, art pipeline)
> lives in `shared/`. Studio-level docs (brand, IP guidelines, art
> bible) live in `docs/`. Feature branches live *within* the monorepo
> (e.g., `feat/constellate-combat-grid`). When a project enters full
> Steam production, it can be promoted to its own repo.

### New facts unlocked vs. Batch 1–2

- **Dropped concept full name**: *Wardens of the Veil* (we only had
  "Wardens" before).
- **Zodiac scope is multi-system**: Western constellations, Western
  birth signs, *and* Chinese zodiac — not just Western.
- **Explicit JRPG references** confirmed: Pokémon, Digimon, Fire
  Emblem, Final Fantasy.
- **Plan deliverables enumerated**: repo structure, one-page brief per
  project, zodiac slotting, sequencing strategy.
- **Repo layout extended**:
  - `games/<name>/` per project
  - `shared/` for cross-project tooling (save format, dialogue parser,
    art pipeline)
  - `docs/` for studio-level docs (brand, IP guidelines, art bible)
  - Feature branches live within the monorepo
  - Projects can graduate to their own repo when they enter full Steam
    production.
- **Sequencing rationale**: prep five, build one at a time.

### Implications for current branch (updated)

- Need to add `shared/` and `docs/` directories, not just `games/`.
- The current `STUDIO-NAME.md` arguably belongs under `docs/` (brand);
  the IP guidelines and art bible should join it there.
- `GAMES.md` at root is fine as a slate index; per-game one-page briefs
  go under `games/<name>/`.
- `references/` (the original-plan transcriptions) can stay where it is
  — it's session scaffolding, not part of the locked plan layout.

---

## Batch 4 — Locked repo tree

The original plan ships an explicit directory tree as the locked layout.
Transcribed verbatim:

```
/home/user/Project-Enigma/
├── games/
│   ├── ember-and-echo/         # Project 1
│   ├── constellate/            # Project 2 (zodiac flagship)
│   ├── chorus/                 # Project 3
│   ├── grafted/                # Project 4
│   └── the-lasting/            # Project 5
├── shared/                     # cross-project tools (save fmt, dialogue, ...)
└── docs/                       # studio-level docs (brand, IP guidelines, ...)
```

### Restructure required on this branch

Current branch state vs. the locked tree:

| Path | Current | Target | Action |
|---|---|---|---|
| `games/ember-and-echo/` | missing | required | create with stub README |
| `games/constellate/` | missing | required | create with stub README |
| `games/chorus/` | missing | required | create with stub README |
| `games/grafted/` | missing | required | create with stub README |
| `games/the-lasting/` | missing | required | create with stub README |
| `shared/` | missing | required | create with stub README |
| `docs/` | missing | required | create |
| `STUDIO-NAME.md` (root) | exists | should live under `docs/` | move to `docs/STUDIO-NAME.md` |
| `GAMES.md` (root) | exists | slate index | keep at root (acts as portfolio overview) |
| `references/` | exists | session scaffolding | keep as-is |

---

## Batch 5 — Studio-wide design rules + start of Project briefs

### Studio-wide design rules (apply to every project)

Reconstructed from full-line stitching across screenshot fragments:

- **Original IP** — original world names, original creature/character
  taxonomy, original visual silhouettes. Where mythologies are
  referenced (zodiacs), [reference but do not appropriate].
- **Avoid Nintendo's recent creature-catching patents** — no
  throw/capture/mount sequence; use **binding, summoning, grafting,
  remembering** instead.
- **Engine: Godot 4** for all projects (free, MIT, 2D-strong, exports
  to Steam + iOS + Android). Avoids Unity's runtime-fee risk and
  Unreal's 2D [pain].
- **Save schema versioned from day one** for every project; supports
  paid chapter expansions without breaking saves.
- **Premium model** across the studio: one-time purchase + paid chapter
  expansions. **No gacha, no FOMO, no live-ops.**
- **Localization-ready** UI strings (translation table) from day one;
  English at launch, community translations later.
- **Pixel art** as default art form (32×32 or 48×48 sprites);
  commission a single character artist per project once prototype
  validates the loop.

### Project briefs — section opens

**1. Ember & Echo — Memory-Bound Tactics** *(lead title)*

- **Folder**: `games/ember-and-echo` / `games/ember-and-echo/`
- **Hook** (partial — ends mid-sentence; needs next batch):
  > In a world where strong memories crystallize into spirit-creatures
  > called **Echoes**, you play a **Reverist** who steps into a
  > person['s memory…]

Subsequent fields (Loop, Hooked-on, Scope, etc.) await the next batch.

### New facts unlocked vs. earlier batches

- **Engine locked: Godot 4** (resolves an open question and overrides
  the assumption I'd been carrying that engine was TBD).
- **Creature interaction verbs** are explicitly *bind / summon / graft
  / remember*, not catch/throw/mount — to dodge Nintendo's patents.
  This directly shapes **Grafted**'s core mechanic (the verb fits) and
  reframes Ember & Echo's "Echoes" as bound/summoned, not captured.
- **Premium-only across the studio**, no gacha. Directly contradicts
  my earlier "Grafted as mobile gacha-adjacent" framing — drop that
  entirely.
- **Ember & Echo's locked subtitle**: *Memory-Bound Tactics* — names
  the genre as a tactics game, not a free-form JRPG.
- **In-fiction proper nouns surfaced**:
  - **Echoes** — spirit-creatures formed from crystallized memories
  - **Reverist** — the player class/role
- **Pixel art locked at 32×32 / 48×48**; single character artist per
  project commissioned only after prototype validation.

### Reconciliation table — updated

| Item | Earlier-session proposal | Original plan | Action |
|---|---|---|---|
| Ember & Echo genre | "narrative JRPG" | **tactics** ("Memory-Bound Tactics") | Use "tactics" as the locked genre |
| Grafted monetization | mobile gacha-adjacent | premium, no gacha, no live-ops | Drop gacha framing entirely |
| Engine | TBD | Godot 4 | Locked |
| Creature mechanic verbs | catch/tame | bind / summon / graft / remember | Use the locked verbs |
| Art style | TBD | pixel art (32×32 or 48×48) | Locked |
| Localization | TBD | EN at launch, community translations later, table from day one | Locked |
