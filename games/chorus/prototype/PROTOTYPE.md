# Chorus — Paper Prototype Brief

*Phase 2. No code. Goal: in 5 minutes of play, decide whether the
two-axis composition system (shape × timbre) produces meaningful
positioning decisions without overwhelming the player.*

## Hypothesis

Combining **adjacency shape** (Solo / Duet / Triad) with **timbre
mix** (Voice / Brass / String / Wind) produces positioning
tradeoffs that feel like *making music*, not like *solving a
spreadsheet*, by turn 3.

## Materials

- 1 sheet of grid paper, 6×6 marked.
- 4 player **Choir cards**, each labeled with a single timbre:
  - Card 1: **Voice** (HP 4, base d6 attack)
  - Card 2: **Brass** (HP 4, base d6 attack)
  - Card 3: **String** (HP 4, base d6 attack)
  - Card 4: **Wind** (HP 4, base d6 attack)
- 3 enemy index cards (HP 4 each, base d6 attack, no chord ability).
- 6 d6 dice.
- HP tokens.
- A printed **chord reference card** (see below).

## Setup

1. Player deploys 4 Choir cards on row 1 of the 6×6 grid.
2. Enemy deploys 3 cards on row 6.
3. The Conductor is **not on the grid** — the player issues moves
   but does not occupy a square.

## Rules — turn structure

Each turn:

1. **Player turn** — pick *one* Choir card and either move it 1
   square (orthogonal) or have it perform a Solo action.
2. **Resolve composition** — count contiguous orthogonally-adjacent
   clusters of Choir cards on the grid:
   - **Solo (1 isolated)** = utility action only (heal 1, defend,
     etc.)
   - **Duet (2 adjacent)** = mid-tier spell (1 die).
   - **Triad (3 adjacent)** = chord; **timbre determines spell**
     (see reference card).
   - **Quartet (4 adjacent)** = extended chord, +1 die over Triad.
3. **Spell resolution** — once per turn, the player declares which
   cluster to "play" and rolls dice as per the chord type. 4+ deals
   1 damage to a chosen target (or AoE per chord rule).
4. **Enemy turn** — each enemy moves 1 square toward the nearest
   Choir card; if adjacent, attacks (d6, 4+ deals 1 damage).

### Chord reference card

```
Cluster size    Timbre mix              Spell
-------------------------------------------------------
Solo (1)        any                     Defend (no damage; +1 HP)
Duet (2)        any                     Riff (1 die, single target)
Triad (3)       all same timbre         Fanfare (3 dice, single)
Triad (3)       all-different timbres   Ballad (2 dice, AoE 2 sq)
Triad (3)       2 same + 1 other        Concerto (2 dice, single + 1 self-heal)
Quartet (4)     any                     Suite (above effect, +1 die)
```

## Success criteria

The prototype passes if:

- **By turn 3**, the player makes a positioning decision driven by
  *which spell they want* (not just by which enemy is closest).
  Typically: "I want a Fanfare next turn, so I'll move Brass over
  to the cluster instead of attacking."
- **Legibility**: by turn 3, the player can name the chord their
  current cluster will produce *without re-reading the reference
  card*.
- **5-minute fun test**: the player wants to play a second battle
  to try a different timbre mix or formation.

If the player keeps re-reading the reference card past turn 3, or
defaults to "always Triad," the system needs simplification.

## What to log

- Time-to-first-formation-driven-move (turn number).
- Whether the player ever tried a Solo or Duet on purpose (vs.
  always defaulting to Triad).
- Reference-card re-reads after turn 3.
- One sentence on whether *naming the chord* felt satisfying.
- One sentence on whether absent Percussion (held back for chapter
  2 in the design doc) was missed.

## Constraints

- No Percussion timbre in this prototype. 4 timbres only.
- No real audio — chord names are spoken aloud.
- No multi-tone characters in this test.
- No story / vignette wrapping. Combat-only.
- Battle ends at first wipe or 6-turn timeout.
