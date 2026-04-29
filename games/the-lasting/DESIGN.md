# The Lasting — Time-Loop JRPG

*v0 design doc — one-page brief per the Phase 1 spec.*

## 3-sentence pitch (verification gate)

You arrived in a small kingdom thirty days before its end, and you
are the only person who remembers each loop ends and begins again.
Combat is ATB-style party RPG with light systems and heavy narrative
weight; the real game is what you piece together about the kingdom,
its twelve recruitable companions, and yourself across cycles. It's
a quietly fatalistic time-loop JRPG where knowledge persists, items
don't — and the catastrophe, you'll eventually learn, is closer to
home than you wanted.

## Hook

You came to the kingdom with a reason. You haven't told anyone, and
you might not yet have admitted it to yourself. Thirty days after
your arrival, the kingdom ends. The next morning is day one again,
and you remember everything. They don't.

## Core loop

1. **Loop opens** — same day-one starting state every cycle.
2. **Live the month** — knowledge from prior loops shapes what you
   can do this loop. Doors open you couldn't open before.
3. **Recruit / re-recruit companions** — meet them, build trust;
   some require specific knowledge to befriend.
4. **Combat encounters** — ATB-style party RPG; combat resolves
   obstacles, doesn't dominate screen time.
5. **Day 30 / catastrophe** — loop closes; reset.
6. **Compound** — each chapter, accumulated knowledge pushes the
   timeline forward or backward and the loop itself starts to bend.

## The loop system — what carries, what resets

| Persists | Resets |
|---|---|
| Knowledge and discovered facts | Items / inventory |
| Map reveal | Equipment |
| Companions you've befriended (no need to redo first-meet) | Active party composition |
| Major story flags | NPC schedules, world state |
| Each companion's **birth-sign signature ability** (one each) | Most other character progression (small carryover for "deeply learned" abilities) |

Design intent:

- **Items reset** to prevent grind-to-power; you cannot farm your way
  past hard fights.
- **Skills mostly reset** to keep early loops scary.
- **Knowledge IS the power** — late loops, you arrive vulnerable
  mechanically but armed with what to do.
- **Signature abilities persist** as the small permanent thing the
  player accumulates — one per companion, unlocked through their
  arc.

## The 12 companions

Twelve recruitable companions, each carrying one of 12 original
birth-sign archetypes (Western-zodiac-inspired but renamed and
redesigned per `docs/IP-GUIDELINES.md`). Each archetype has a
baseline loop-reaction stance; specific characters within an
archetype can subvert it.

| Loop reaction | Count | Behavior |
|---|---|---|
| **Fatalistic** | ~4 | Accept the loop. Find peace, art, or routine within it. |
| **Defiant** | ~4 | Refuse the loop. Push for permanent change at any cost. |
| **Scheming** | ~4 | Leverage the loop for personal goals; some have hidden agendas. |

Each companion ships with:

- A **signature ability** (the only mechanical thing that persists
  across loops once unlocked).
- A **personal arc** that can resolve or transform across cycles.
- **Support conversations** gated by knowledge, companions present,
  and loop-count.
- **Story branches** affected by their presence/absence in the party.

The 12 are not all available in a single loop. Some require
knowledge from prior cycles to even meet. A full roster is **found
across multiple loops**, then assembled into a "knowing" loop.

## Original IP

The kingdom, its cosmology, the catastrophe's nature, the 12 birth-
sign archetypes (with original names), the loop's cosmological
cause, and every named companion are original to Cleave Studios.
Zodiac references are deliberately *light* and *narrative-flavored*
rather than system-defining — Constellate carries the studio's
mechanical-zodiac load (see `games/constellate/DESIGN.md`); The
Lasting carries the *characterological* one. The two zodiac games
stay clearly distinct.

## Episodic plan

Each chapter breaks more of the loop or extends the timeline.
Chapter pivots are knowledge-revelations.

| Chapter | Loop state | Revelation |
|---|---|---|
| 1 | First few loops | Kingdom dies day 30. Catastrophe shape unclear. |
| 2 | First 3–4 companions met; loop dynamics learned | Catastrophe has a *direction* — something specific is happening. |
| 3 | Loop start can be pushed earlier (timeline extends backward) | Earlier day-one reshapes what the catastrophe looks like. |
| 4 | More companions; political layer of the kingdom revealed | The catastrophe involves the protagonist's purpose for coming. |
| 5 | All 12 companions findable; the "knowing" loop | Catastrophe revealed in full — it's tied to you. |
| 6+ | Endgame loops | Choose to break forward, break backward, or stay. |

Paid chapter expansions can ship a 13th sign, or extend the timeline
further past / future to open new arcs.

## V-slice scope (Phase 3 target)

Per the original plan: **1 hub, 1 vignette, 1 battle, 4 starters,
1 evolution event. ~30 min of polished play.**

- **Hub**: a single corner of the kingdom on day-one of the
  protagonist's first arrival — a market square or inn. One walkable
  area, three or four NPCs.
- **Vignette**: meet the first companion; learn the rhythm of the
  day cycle.
- **Battle**: one ATB-style 4-character encounter that resolves a
  small obstacle and demonstrates combat pace + narrative
  integration.
- **Starters**: the protagonist + three companions covering one
  fatalist, one defiant, one schemer — teaches the archetype
  spectrum on day one.
- **Evolution event**: **the first loop reset itself.** The
  catastrophe happens (a lighter foreshadow of its full form), day-
  one returns, and the player retains knowledge while every NPC
  resets. The V-slice's payoff moment is the entire game's thesis.

Verification: ≥40% itch.io demo completion + ≥60% "would buy" signal
on the V-slice.

## Tone

*Outer Wilds*-grade quietly fatalistic with wonder. Acceptance over
urgency. Mortality without grimdark. The kingdom is beautiful in
ways the player only learns to see because they have time to look.
Music sparse and ambient; long silences are tonal, not technical.

## Strategic role

- The slate's **narrative anchor** — heaviest writing investment per
  hour of player time.
- **Light system focus** means it's relatively cheap to ship
  mechanically — good shape for the back half of a solo-dev career.
- **Replay value** via different party compositions and endings
  (break forward / break backward / stay).
- **Strong audience match** with the time-loop genre cohort (Outer
  Wilds, 12 Minutes, In Stars and Time, Sea of Stars).
- **Risk**: narrative-heavy means the writing has to land. Less
  forgiving than the system-driven titles on the slate.

## Open questions for paper-prototype phase

- 30-day cycle length — is 30 too long for a tractable loop, too
  short for meaningful kingdom-life beats? What's the right tick
  rate (in-game hours per real-time minute)?
- 12 companions — is that too many for a solo-dev narrative budget?
  Could the slate ship at 8 with the other 4 in a paid expansion?
- Birth-sign signature abilities — how distinct can 12 feel
  mechanically when they're the only persistent carryover, without
  duplicating Constellate's job-class system?
- The "personal-and-cosmic" reveal — is the protagonist-as-cause
  twist powerful enough to anchor 20+ hours of play, or does it
  need a second narrative engine to share the load?
- Loop-count visibility — does the player see a counter, or stay
  in the dark? Both have precedent.
- Items reset — does it feel punitive or freeing in playtest? At
  what point in a loop does it stop hurting?
