# Chorus — Music-Powered Tactical RPG

*v0 design doc — one-page brief per the Phase 1 spec.*

## 3-sentence pitch (verification gate)

You play a mute conductor walking a world rebuilding from **the
Hush** — the silencing of the World-Song that once held reality
together. Combat is FE-style grid tactics where you compose magic by
arranging your **Choir**: adjacency on the grid forms the chord
shape, and the tones (Voice, Brass, String, Wind, Percussion) of who
clusters together set its timbre. It's positioning-as-music in a
bardic-folk JRPG that walks region by region through reclaimed
musical genres.

## Hook

Once, a continuous music called the **World-Song** held reality
together. Then the Hush silenced it, and the world began to fray —
coastlines unraveling, cities forgetting their names, mornings that
don't quite arrive. You walk between what's left, conducting a Choir
of voices and instruments. You cannot sing. You cannot play. But you
can place each voice on the ground beside another, and where they
meet, the music returns.

## Core loop

1. **Region travel** — walk into a new region tied to a musical
   genre and a faction.
2. **Choir recruitment** — meet voices and instruments; bind them
   into the Choir through one-screen vignettes.
3. **Tactical battle** — FE-style grid. The Conductor moves like any
   other unit but cannot directly attack; combat resolves through
   the Choir's composed chords.
4. **Composition mastery** — each region teaches a new chord shape,
   timbre family, or compositional rule unique to its tradition.
5. **World-repair narrative** — clearing each region literally
   re-stitches a verse of the World-Song. The map heals as you play.

## The composition system — two axes

Compose magic by managing **shape** (adjacency pattern) and
**timbre** (which tones cluster).

### Shape — adjacency on the grid

| Adjacent units | Form | Tier |
|---|---|---|
| 1 | Solo | Utility / status |
| 2 | Duet | Mid-tier spell |
| 3 | Triad | Base chord — primary spell tier |
| 4 | Quartet | Extended chord |
| 5+ | Suite | Rich chord — ultimate-tier |

Adjacency is orthogonal (no diagonals).

### Timbre — five tone families

Every Choir member carries one tone (a few rare members carry two):
**Voice, Brass, String, Wind, Percussion.**

The mix of tones in a chord sets its quality. Examples:

- All-Brass → **Fanfare** (aggressive single-target damage)
- All-Voice → **Aria** (high single-target burst)
- All-Percussion → **Drumline** (party mobility / positioning)
- Voice + String + Wind → **Ballad** (balanced AoE)
- All-different → **Concert** (utility / area control)

Specific chord-family names, exact spell mappings, and the full
chord-quality matrix are reserved for `LORE.md`, `CREATURES.md`, and
the paper-prototype phase.

## Original IP

The mute-conductor protagonist, the Choir, the Hush, the World-Song,
the three named factions (Brass City, Stringfen, the Silent Order),
and the two-axis composition system are original to Cleave Studios.
Music as a concept isn't ownable, but every faction, chord-family,
region-genre, world-repair beat, and timbre nomenclature is. See
`docs/IP-GUIDELINES.md`.

## Episodic plan

Each chapter = a new region tied to a musical genre and a faction.

| Chapter | Region (placeholder) | Faction stance | Teaches |
|---|---|---|---|
| 1 | Tutorial valley | Independent | Folk genre; Solo / Duet / Triad shapes |
| 2 | Brass City outskirts | Brass City rival | Marches and fanfares; Brass-heavy timbre |
| 3 | Stringfen lowlands | Stringfen ally | String quartets and ballads |
| 4 | Silent Order territory | Silent Order antagonist | Forbidden chords; constrained-tone combat |
| 5+ | Re-coalescence of the World-Song | All factions in conflict | Mixed-timbre Suites; multi-region puzzles |

Paid chapter expansions can add musical traditions outside the
launch slate (e.g., jazz, religious choral, percussion-only) with
new chord families exclusive to that DLC.

## V-slice scope (Phase 3 target)

Per the original plan: **1 hub, 1 vignette, 1 battle, 4 starters,
1 progression event. ~30 min of polished play.**

- **Hub**: the tutorial valley village. One walkable street, one
  mentor figure who hands the player the conductor's role.
- **Vignette**: assemble the first triad — meet three Choir members
  in three short scenes, place them adjacent for the first time,
  hear the chord.
- **Battle**: one FE-style grid encounter. 4 Choir members vs. an
  early World-Song fray. Teaches Solo, Duet, Triad shapes with two
  different timbre mixes.
- **Starters**: four Choir members covering four of the five timbres
  (Voice, Brass, String, Wind). Percussion deliberately held back
  for chapter 2 to give the player a "first new tone" reveal.
- **Progression event**: one Choir member gains a second tone mid-
  battle (e.g. a Voice becomes Voice/String), teaching the
  multi-tone mechanic and previewing build depth.

Verification: ≥40% itch.io demo completion + ≥60% "would buy" signal
on the V-slice (per `references/original-plan.md` Verification gates).

## Tone

*Octopath Traveler / Bravely Default*-grade storybook-folk. Bardic,
hopeful, episodic. Acoustic-forward sound design — no big synth
textures. Each region has a distinct musical-genre signature, so the
soundtrack itself becomes a gameplay primer.

## Strategic role — marketing edge

Per the original plan, Chorus has the **lowest competition in its
niche** and an **audio-forward identity that's highly shareable on
TikTok/streams**. Implementation implications:

- Combat actually plays back the chord that was composed (real audio
  assets, not just SFX). Every battle is a small recital.
- Each region's musical genre creates distinct shareable clip
  formats — a triad-march clip looks and sounds different from a
  string-ballad clip.
- The bardic-folk tone keeps the audience door wide; not gated
  behind grimdark or anime-bright.

This is the slate's most cuttable-into-30-second-clips title and the
strongest viral marketing surface among the five.

## Open questions for paper-prototype phase

- Does the two-axis system (shape × timbre) stay legible without
  becoming a spreadsheet? At what party size does tone-tracking
  break down?
- Real audio playback of composed chords — does it slow combat
  pacing, or does it accelerate it by giving players an extra
  feedback channel?
- How distinct can the five timbres feel without one dominating in
  the meta?
- The Silent Order chapter (combat without music) — is that an
  interesting forced-handicap puzzle, or does it break the core
  loop and feel like an anti-fun chapter?
- How does the mute-conductor protagonist participate emotionally in
  story scenes without a voice? What's the dialogue convention?
