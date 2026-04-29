# Grafted — Paper Prototype Brief

*Phase 2. No code. Goal: in 5 minutes of play, decide whether
crafting decisions made BEFORE combat produce meaningful tactical
decisions DURING combat.*

## Hypothesis

A 5-slot crafted creature, built in 60 seconds at the bench from a
small parts catalog, plays *visibly differently* from a stock
creature in the same 3v3 row-position combat, and the difference
is felt by turn 3.

This prototype tests **the bridge between craft and combat** — the
single most load-bearing claim of the design.

## Materials

- A **parts catalog** — 12 parts cards, divided as:
  - 3 **Heads** (Mire-aquatic / Forge-volcanic / Wood-symbiotic),
    each grants 1 trained-move family.
  - 3 **Torsos** (one per biome), each sets HP (Mire 5 / Forge 6 /
    Wood 4) and armor (Mire 0 / Forge 1 / Wood 0).
  - 3 **Limb pairs** (one per biome), each sets row-shift speed
    (Mire fast / Forge slow / Wood medium).
  - 3 **Organs** (one per biome) granting 1 innate move:
    - Mireling venom gland → **Toxic** (1 extra damage over time).
    - Forge-finch lung → **Combustion** (deal 1 damage to flanker
      enemies on hit).
    - Whisperwood seed → **Symbiosis** (heal 1 self on attack).
- An **affinity card** for each biome (Mire / Forge / Wood) — the
  player picks one to designate dominant biome.
- 3 player creature templates (5 slot frames each).
- 3 enemy index cards (preset stock creatures, HP 5, base d6).
- 6 d6 dice and HP tokens.

## Setup

### Phase A — Bench (target 90 seconds)

1. Player has 3 creature templates with **2 random pre-filled slots
   each** (acts as a starting roster).
2. Player draws **5 parts** at random from the catalog.
3. Player slots parts onto templates, filling open slots. Goal: at
   least one creature should reach a **purebred bonus** (3+ same-
   biome parts → +1 die on all attacks for that creature) or a
   **named hybrid** (cross-biome organ + matching head — adapter
   logic deferred for v0 prototype).
4. Player declares each creature's **affinity** (biome).
5. Player names each creature on the card.

### Phase B — Combat (target 3-4 minutes)

1. Each creature occupies a row position: **front / back / flank**.
2. Front-line creatures attack the enemy front. Back-line creatures
   attack any enemy but do -1 damage. Flank creatures attack the
   enemy back row directly but take +1 damage.
3. Each turn: player chooses one creature to act (attack with
   trained-move OR innate-move; or shift row).
4. Enemies act in a fixed pattern (Front attacks player Front;
   Flank attacks player Back).
5. Roll dice; 4+ deals 1 damage. Apply innate-move effects.

## Success criteria

The prototype passes if:

- **By turn 3 of combat**, the *crafted* creature plays observably
  differently from the two stock creatures — typically: an innate
  move triggers, a purebred bonus die hits, or an affinity rule
  changes the enemy's targeting.
- **The bench phase took under 2 minutes** but the player still
  felt they made a real choice. (If it took 5 minutes, the catalog
  is too rich; if it took 30 seconds, it's too thin.)
- **5-minute fun test**: at the 5-minute mark (across both phases),
  the player wants to redo the bench with a different parts mix.

If the crafted creature plays identically to a stock one, or the
bench felt arbitrary, the slot-and-symbiosis system isn't earning
its complexity.

## What to log

- Bench phase time (target 60–120 seconds).
- Whether the player chose a purebred build or a hybrid.
- The first turn at which the crafted creature's design choice
  visibly mattered (target: turn 3 or earlier).
- Whether the player named their creature (signal of investment).
- One sentence on whether they wanted to keep this creature or
  rebuild.

## Constraints

- No adapter parts in this prototype. Conflict-pair mechanic is a
  Phase 3+ refinement.
- No procedural sprite generation — index cards only.
- No biome-unlock progression. Single 12-part catalog.
- No faction / story wrapper.
- Combat ends at first wipe or 6-turn timeout.
