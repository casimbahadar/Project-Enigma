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

---

## Batch 6 — Ember & Echo full brief + Constellate opening

### 1. Ember & Echo — Memory-Bound Tactics *(lead title)*

- **Folder**: `games/ember-and-echo` / `games/ember-and-echo/`
- **Hook**: In a world where strong memories crystallize into
  spirit-creatures called **Echoes**, you play a **Reverist** who steps
  into a person's memory and binds the Echo born from it.
- **Core loop**: Tactical-grid combat (FE-style, 4–6 Echoes, 8×8 grid,
  3–7 min battles) → **Resonance system** (adjacent Echoes with
  matched/complementary emotions get buffs) → Echoes evolve along
  branches driven by which emotion-fragments you feed them.
- **Original IP**: Every Echo has a named human origin and a one-screen
  recruitment vignette. Bonds unlock support conversations.
- **Why it's the lead**: Hits all four reference touchstones (FF
  narrative, FE tactics, Pokémon collection, Digimon evolution).
  Captures the "emotions as party characters" intuition exactly.
- **Episodic fit**: Each chapter = a region tied to a memory-theme
  (joy, grief, etc.); new Echoes per chapter.

### 2. Constellate — Star-Forged Companions *(zodiac flagship)* — partial

- **Folder**: `games/constellate` / `games/constellate/`
- **Hook**: A world fragmented into floating sky-isles, each under a
  different celestial sign. **Asterix** creatures are born when
  starlight imprints on living matter. You are a **Stargazer** who maps
  constellations to summon and bond them.
- **Core loop**: ATB-style 4v4 party combat with **zodiac synergies**
  between adjacent party slots. Sky alignment shifts in-game weekly,
  rotating which celestial signs are dominant — natural daily/weekly
  meta on mobile, scheduled boss windows on Steam.
- **Three-tier celestial cosmology** (uses all the zodiac flavors):
  - **The Greater Constellations** (12+ original constellations) →
    creature *families* with their own mythology.
  - *(remaining tiers TBD in next batch)*

### New facts unlocked

- **Ember & Echo's full mechanic stack**:
  - Genre: tactical-grid (FE-style)
  - Party size: 4–6 Echoes
  - Grid: 8×8
  - Battle length: 3–7 min
  - **Resonance system** for adjacency buffs
  - Echo evolution branches driven by emotion-fragment feeding
  - Recruitment via memory-vignettes + bonds-unlock-supports
  - Chapter structure = regions tied to memory-themes

- **Constellate's in-fiction terms**:
  - **Asterix** = creature class (starlight on living matter)
  - **Stargazer** = player class
  - World shape: floating sky-isles per celestial sign
  - **Three-tier cosmology** structure (only top tier visible so far —
    "Greater Constellations" with 12+ originals)

- **Potential design tension to flag**:
  - Studio-wide rule (Batch 5): "No gacha, no FOMO, no **live-ops**."
  - Constellate brief: "daily/weekly meta on mobile, scheduled boss
    windows on Steam."
  - These read as adjacent — rotating-content-as-natural-meta vs.
    operator-driven live-ops — but worth surfacing as a question if/when
    we deep-dive Constellate.

- **Ember & Echo recruitment language**:
  - The verb is **bind** (matches the "bind / summon / graft / remember"
    list from Batch 5's no-Nintendo-patent rule).

---

## Batch 7 — Constellate (full), Chorus, Grafted

### 2. Constellate — Star-Forged Companions *(zodiac flagship)* — FULL

- **Folder**: `games/constellate` / `games/constellate/`
- **Hook**: A world fragmented into floating sky-isles, each under a
  different celestial sign. **Asterix** creatures are born when
  starlight imprints on living matter. You are a **Stargazer** who maps
  constellations to summon and bond them.
- **Core loop**: ATB-style 4v4 party combat with **zodiac synergies**
  between adjacent party slots. Sky alignment shifts in-game weekly,
  rotating which celestial signs are dominant — natural daily/weekly
  meta on mobile, scheduled boss windows on Steam.
- **Three-tier celestial cosmology** (uses all the zodiac flavors):
  - **The Greater Constellations** (12+ original constellations) →
    creature *families* with their own mythology.
  - **The Birth Signs** (12 original signs, Western-zodiac-inspired
    but renamed) → the player's chosen birth sign sets a starter
    Asterix and an innate ability (FF job-class equivalent).
  - **The Beast Court** (12 original spirit-beasts,
    Chinese-zodiac-inspired but renamed and redesigned) → faction
    leaders who govern world regions; aligning with one unlocks story
    branches and exclusive Asterix.
- **Original IP**: Fully owned celestial pantheon. Names and visual
  silhouettes are original; archetypes only gesture at known zodiacs
  (e.g., a horned charging beast in place of Aries).
- **Episodic fit**: Each new chapter = a new sky-isle + new
  constellation + new Beast Court allegiance branch.

### 3. Chorus — Music-Powered Tactical RPG

- **Folder**: `games/chorus` / `games/chorus/`
- **Hook**: After "**the Hush**," sound is sacred and songs literally
  power magic. Your party is a **Choir**; each member is a voice or
  instrument; adjacency on the grid composes harmonies that fuel
  combos.
- **Core loop**: FE-style grid combat. Adjacent party members compose
  a chord; chord type unlocks that turn's spells. **Positioning *is*
  the magic system.**
- **Original IP**: Original musical-themed factions (**Brass City**,
  **Stringfen**, **the Silent Order**). Original cosmology of how the
  Hush happened and what music-magic costs.
- **Episodic fit**: Each chapter = a new region tied to a musical
  genre/faction.
- **Marketing edge**: audio-forward identity is highly shareable on
  TikTok/streams; lowest competition in this niche.

### 4. Grafted — Build-A-Beast Bio-punk RPG

- **Folder**: `games/grafted` / `games/grafted/`
- **Hook**: A bio-punk world where **Grafters** splice creature parts
  to create new beings. You don't catch creatures — you **build** them
  from essences harvested from defeated beasts.
- **Core loop**: Party combat with creatures you designed. Each
  creature has trained moves *plus* innate moves inherited from the
  organs you grafted ("venom gland from the **Mireling**" → Toxic).
  **Crafting depth is the meta loop.**
- **Original IP**: Ethical-faction war (**the Pure Strain Order** vs.
  **the Grafter's Guild**) provides narrative spine. Original parts
  catalog and biome ecology.
- **Episodic fit**: Each chapter = a new biome with a new parts
  catalog.
- **Marketing edge**: every player's roster looks unique → natural
  sharing/screenshot engine.

### New facts unlocked in Batch 7

**Constellate — full cosmology**:
- All three zodiac systems are mapped to discrete in-game tiers:
  - Greater Constellations → creature *families* + mythology (top tier)
  - Birth Signs → 12 originals, Western-zodiac-inspired, drives starter
    Asterix + innate ability (FF job-class equivalent)
  - Beast Court → 12 originals, Chinese-zodiac-inspired, drives
    faction leaders + region politics + exclusive recruits
- All names/silhouettes are original; archetypes only *gesture* at
  known zodiacs (Aries → horned charging beast, etc.) — explicit
  rule for original-IP integrity.

**Chorus — locked terms**:
- World event: "**the Hush**"
- Party: **Choir**
- Factions: **Brass City**, **Stringfen**, **the Silent Order**
- Magic system thesis: positioning on the grid *is* the magic
- Marketing claim: lowest-competition niche; TikTok-friendly identity

**Grafted — locked terms**:
- Player class: **Grafters**
- Verb: **build** (not catch) — matches the "build/graft" verbs from
  the Nintendo-patent-avoidance rule
- Factions: **the Pure Strain Order** (ethical opposition) vs. **the
  Grafter's Guild** (player-aligned)
- Example creature: **Mireling** (its venom gland → Toxic affinity)
- Meta loop: crafting depth, not collection breadth
- Episodic structure: chapter = biome + parts catalog
- Marketing claim: every roster is unique → screenshot/share-driven
  reach

**Cross-cutting observations**:
- The "no Nintendo patents" rule is honored verb-by-verb across the
  slate: *bind* (E&E), *summon* (Constellate), *compose* (Chorus —
  positioning-as-magic), *build/graft* (Grafted).
- Each game has a single sentence that names its **meta loop** /
  identity claim — useful spine for marketing copy.
