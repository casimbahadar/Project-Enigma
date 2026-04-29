# Ember & Echo — Paper Prototype Brief

*Phase 2. No code. Goal: in 5 minutes of play, decide whether the
Resonance system produces meaningful tactical decisions.*

## Hypothesis

Adjacency-based emotion **Resonance** on an 8×8 grid creates a real
positioning tradeoff — moving for damage *now* vs. moving for a
Resonance pair *next turn* — that becomes interesting by turn 3.

## Materials

- 1 sheet of grid paper, 8×8 marked (or a chessboard).
- 8 index cards labeled as Echoes: 4 player, 4 enemy. On each,
  write: name, base emotion (Joy / Grief / Anger / Fear / Longing /
  Resolve), HP (4), basic attack die (d6).
- 6 d6 dice.
- A small pile of HP tokens (pennies, paper clips).

## Setup

1. Player deploys 4 Echoes on row 1; enemy deploys 4 on row 8.
2. Pick starting emotions for the 4 player Echoes: **Grief, Longing,
   Resolve, Anger** (gives one Resonance pair available — Grief+
   Longing — and one clash — Anger ↔ Joy among enemies).
3. Enemy emotions: **Joy, Fear, Anger, Grief**. Vary if you want a
   second test run.

## Rules — turn structure

Each turn, in order:

1. **Player turn** — pick *one* Echo and either move it 1 square
   (orthogonal only) or attack an adjacent enemy.
2. **Resolve Resonance** — for each player Echo, check its 4
   orthogonal neighbors. If any neighbor is also a player Echo with
   a wheel-adjacent or matching emotion, this Echo's next attack is
   **+1 die**. Opposite emotion neighbor = **-1 die**.
3. **Attack resolution** — roll the appropriate dice (modified by
   Resonance), each 4+ deals 1 damage.
4. **Enemy turn** — same rules, enemy moves toward closest player
   Echo and attacks if adjacent.

### Emotion wheel (clockwise)

`Joy → Resolve → Anger → Grief → Longing → Fear → Joy`

- **Adjacent on wheel** = Resonance buff.
- **Opposite** (Joy↔Grief, Resolve↔Longing, Anger↔Fear) = clash
  debuff.
- **Identical** (two Joys) = mild echo amp (+1 die only when
  attacking the *same* target as your twin).

## Success criteria

The prototype passes if:

- **By turn 3**, the player faces a non-trivial composition decision
  — typically: "do I move Grief next to Longing for the Resonance
  buff, or do I move Grief into attack range of an enemy *now*?"
- **5-minute fun test**: at the 5-minute mark, the player wants to
  start a new battle with a different Echo composition.
- **Legibility**: the player can predict the Resonance state of the
  next turn without re-reading the wheel.

If the decision tree feels obvious or the player doesn't try a new
composition on a second run, the system needs revision.

## What to log

- Time-to-first-Resonance-decision (turn number).
- Number of times the player moved *for positioning* vs. *for attack*.
- Any moment where the wheel was re-checked (suggests legibility
  problem).
- One sentence on whether the player wanted to play again.

## Constraints

- No Echo evolution, no support conversations, no story vignette.
  Combat-only test.
- No Shades, no Compound emotions. Run-1 system only.
- Battle ends at first faction wipe or 8-turn timeout, whichever
  comes first.
