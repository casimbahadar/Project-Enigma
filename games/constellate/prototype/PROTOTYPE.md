# Constellate — Paper Prototype Brief

*Phase 2. No code. Goal: in 5 minutes of play, decide whether ATB
4v4 with adjacency synergy stays legible without becoming a
spreadsheet.*

## Hypothesis

A **4v4 party line** where each Asterix has a Birth Sign and a
Greater Constellation family, and where slot adjacency creates
synergy buffs, produces meaningful slot-order decisions by turn 3
without requiring the player to track more than two synergy rules
at once.

## Materials

- 12 index cards as **Asterix cards**. On each: name, Birth Sign
  (use 4 placeholder signs A/B/C/D), Greater Constellation family
  (use 3 placeholder families X/Y/Z), HP (5), attack die (d6),
  one signature ability sentence.
- 4 enemy index cards (HP 5, attack die d6, no synergy).
- 6 d6 dice.
- HP tokens.
- A printed "synergy reference card" (see below) — one for the
  player, one for the runner.

## Setup

1. Pick **4 of 12** Asterix cards for the player. Lay them in a
   row, slot 1 → slot 4.
2. Lay 4 enemy cards opposite.
3. Each Asterix in slot N is **adjacent** to slots N-1 and N+1
   (slots 1 and 4 each have only one neighbor).

## Rules — turn structure

Combat is **ATB-by-initiative**:

1. At the start of each round, every Asterix and enemy rolls 1d6.
   Resolve actions in **lowest-to-highest** order.
2. On its turn, an Asterix can **attack** (the enemy in its slot's
   column — slot 1 attacks enemy slot 1, etc.) or **swap** with an
   adjacent slot (uses the turn).
3. **Synergy resolution** — before an Asterix attacks, check both
   neighbors:
   - **Same Birth Sign as a neighbor** → +1 attack die.
   - **Same Greater Constellation family as a neighbor** → +1
     attack die.
   - **Opposite Birth Sign as a neighbor** (A↔C, B↔D) → -1 attack
     die.
4. Each 4+ on a die deals 1 damage.

### Synergy reference card

```
Birth Signs: A, B, C, D    (opposites: A↔C, B↔D)
Constellation families: X, Y, Z    (no opposites)
Adjacent same-Sign     → +1 die
Adjacent same-Family   → +1 die
Adjacent opposite-Sign → -1 die
Stacking allowed (max +2 dice from neighbors)
```

## Success criteria

The prototype passes if:

- **By turn 3**, the player makes a deliberate **swap** to set up a
  synergy chain — typically: "if I swap slot 2 and 3, my slot-3
  Asterix gets +2 dice next turn."
- **Legibility**: the player can compute their attack die count
  without re-reading the synergy card after turn 3.
- **5-minute fun test**: the player wants to try a different 4-card
  draft on a second run.

If the player is computing dice slowly past turn 3, or never makes a
slot swap, the synergy rules need pruning.

## What to log

- Time-to-first-swap (turn number).
- Number of times the synergy reference card was re-read after
  turn 3 (suggests legibility problem).
- Whether the same draft was used twice or the player tried a new
  4-card draft.
- One sentence on whether two simultaneous synergy axes (Sign +
  Family) felt rich or overwhelming.

## Constraints

- No Beast Court allegiance. No sky alignment. No three-tier
  cosmology surfacing in this test — only **slot adjacency
  synergy**.
- No movement / repositioning beyond the swap action.
- Signature abilities are written on cards but **not used** in this
  prototype unless time permits a second-pass test.
- Battle ends at first wipe or 6-turn timeout.
