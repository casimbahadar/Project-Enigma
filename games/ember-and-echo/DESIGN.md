# Ember & Echo — Memory-Bound Tactics

*Lead title. v0 design doc — one-page brief per the Phase 1 spec.*

## 3-sentence pitch (verification gate)

You play a veteran Reverist who steps into a person's memory and
binds the spirit-creature it crystallizes into — an **Echo**. Combat
is 8×8 FE-style grid tactics where adjacent Echoes resonate by
emotion: matched and complementary feelings buff, opposites clash.
It's emotions as party characters in a quietly grieving JRPG; the
campaign opens with your mentor's last memory.

## Hook

In a world where strong memories crystallize into spirit-creatures
called Echoes, the Reverist trade is a kind of psychopomp work —
stepping into a memory, finding the Echo born from its emotional
charge, and binding it before it dissolves. You play a veteran
Reverist carrying one memory you have never been able to bind: your
own. The campaign begins when your mentor dies and leaves you their
last memory to enter.

## Core loop

1. **Memory-dive vignette** — one-screen scene where you encounter an
   Echo and learn its named human origin. Choose how to engage:
   listen, push, refuse. The choice biases the Echo's starting
   emotion-fragment.
2. **Tactical battle** — 8×8 grid, FE-style. 4–6 Echoes per side.
   3–7 minute encounters. Win conditions vary by memory (rout, escort,
   protect a remembered object).
3. **Resonance** — adjacent Echoes with matched or wheel-adjacent
   emotions buff each other; opposites clash and debuff. Positioning
   is the system.
4. **Evolution** — between battles, feed an Echo emotion-fragments
   harvested from beaten foes. The fragment-mix determines which
   branch the Echo grows along; this is permanent for that Echo.
5. **Bond / support** — passing affinity thresholds with an Echo
   unlocks one-screen support conversations that re-route subsequent
   vignettes.

## Resonance — three layers

- **Run 1 (standard) — 6 base emotions on a wheel**: Joy, Grief,
  Anger, Fear, Longing, Resolve. Adjacent = buff, opposite = clash,
  same-twice = mild echo amp. Teachable in two battles.
- **Late Run 1 unlock (Chapter 4–5) — Shades**: each base splits into
  two (e.g. Joy → Elation / Contentment). Wheel grows to 12 points.
  Same-base shades pair stronger than two generic same-base; new
  cross-shade combos open. Story beat tied to the veteran Reverist's
  sharpening perception.
- **NG+ ("Echoed Heart") and harder modes — Compound emotions**:
  Bittersweet (Joy+Grief), Restless (Fear+Anger), etc. — Echoes whose
  alignment is intrinsically the Resonance buff in creature form.
  Optional, reserved for mastery play.

## Original IP

Reverists, Echoes, the **bind**-into-memory verb, and the Resonance
taxonomy are original to Cleave Studios. No element is derivative of
Pokémon, Digimon, MTG, or other creature-collector franchises. Every
Echo carries a named human origin and a one-screen recruitment
vignette — the IP is *what each Echo remembers*, not a generic
type-chart. See `docs/IP-GUIDELINES.md`.

## Episodic plan

Each chapter is a region tied to one of the six base emotions; the
opening arc walks the wheel.

| Chapter | Theme | Setting (placeholder) |
|---|---|---|
| 1 | Grief | Lakeside village; the mentor's last memory |
| 2 | Anger | TBD — borderland or contested town |
| 3 | Longing | TBD — wilderness / frontier |
| 4 | Fear | TBD — urban / interior |
| 5 | Joy | TBD — festival or celebration; **Shades unlock** |
| 6 | Resolve | TBD — climax; the Reverist's own un-bindable memory |

Each chapter yields new Echoes with that chapter's emotional
signature. Paid chapter expansions can add deeper themes
(e.g. Compound-emotion expansion for the NG+ audience).

## V-slice scope (Phase 3 target)

Per the original plan: **1 hub, 1 vignette, 1 battle, 4 starters,
1 evolution event. ~30 min of polished play.**

- **Hub**: the lakeside village; one walkable street, one talkable
  villager who hooks the player into the mentor's memory.
- **Vignette**: enter the mentor's last memory; discover the Echo;
  choose how to engage (listen / push / refuse).
- **Battle**: one 8×8 grid encounter inside the memory. 4 starter
  Echoes vs. an opposing emotional charge.
- **Starters**: four Echoes covering four base emotions — **Grief,
  Longing, Resolve, Anger** — chosen so the player gets a Resonance
  pair (Grief + Longing) and a clash option (Anger ↔ ???) on turn 1.
- **Evolution event**: one starter Echo branches based on the
  emotion-fragments collected in battle.

Verification: ≥40% itch.io demo completion + ≥60% "would buy" signal
on the V-slice (per `references/original-plan.md` Verification gates).

## Tone

*Lost Odyssey / FF X*-grade quietly grieving. Restrained, mythic,
warm. Memory-dives have the hush of a chapel; combat has the
clean pulse of a tactics game. No anime-bright; no grimdark.

## Why this is the lead

Hits all four reference touchstones in one game: FF narrative, FE
tactics, Pokémon-style collection (every Echo is a named individual),
Digimon-style branched evolution. Captures the "emotions as party
characters" intuition exactly. Smallest believable scope for a
solo-dev tactics RPG that still expresses the studio identity.

## Open questions for paper-prototype phase

- Does Resonance stay legible at 4 Echoes on an 8×8 grid, or does it
  need 6 to feel rich?
- How long should a single battle run? Plan says 3–7 min — the
  prototype should narrow this.
- Does the Shade-unlock land at chapter 4 or chapter 5? Pacing test.
- What's the ratio of memory-dive minutes to tactical-battle minutes
  per hour of play? Target: roughly 40/60.
