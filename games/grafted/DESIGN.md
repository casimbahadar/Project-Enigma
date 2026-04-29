# Grafted — Build-A-Beast Bio-punk RPG

*v0 design doc — one-page brief per the Phase 1 spec.*

## 3-sentence pitch (verification gate)

You play a renegade from the **Pure Strain Order**, forced to learn
the craft you were raised to oppose: grafting harvested parts onto
bench creatures to build new beings. Combat is 3v3 turn-based with
front/back/flank row positions, and every fighter on the field is a
creature you designed — its trained moves layered with innate moves
inherited from the organs you grafted in. It's a bio-punk RPG where
each player's roster looks unmistakably theirs, and the ethical-
faction war is something you carry into the workshop yourself.

## Hook

You were raised by the Pure Strain Order to believe creatures are
sacred as their birth biomes made them — that grafting is violence
dressed up as craft. Then your circumstances changed, and the only
people who would take you in were the **Grafter's Guild**. Now you
stand at a bench cutting harvested parts free of one beast and
binding them into another, and you find — against your will — that
you are good at it. Each creature you build is yours. Each one is
also a question you cannot stop asking.

## Core loop

1. **Field expedition** — venture into a biome, defeat hostile
   beasts, harvest parts.
2. **Workshop / bench** — return to the Guild, slot harvested parts
   onto your roster. Resolve adapter conflicts. Name your creatures.
3. **Combat** — 3v3 turn-based with front/back/flank row positions.
   Trained moves come from the head; innate moves come from the
   grafted organ. Positioning gates targeting and damage falloff.
4. **Faction politics** — the Pure Strain Order pursues; Guild
   internal politics divide; allegiance shifts have story
   consequences.
5. **Biome unlock** — each chapter opens a new biome with a new
   parts catalog and new symbiosis options.

## The grafting system — slots and biome symbiosis

Every crafted creature has **5 slots**:

| Slot | Sets | Notes |
|---|---|---|
| Head | Trained-move tree | The creature's "class" |
| Torso | HP / armor profile | Determines durability shape |
| Limbs (paired) | Mobility / row-shift speed | Front-line vs. flank-suited |
| Organ (one internal) | One innate move | E.g., Mireling venom gland → Toxic |
| Affinity | Dominant biome essence | Symbiosis backbone |

### Biome symbiosis

- **Purebred bonus**: same-biome parts in multiple slots stack into
  meaningful damage / resistance bonuses.
- **Hybrid potential**: mixed biomes unlock unusual types and rare
  innate-move combinations, but at lower individual symbiosis tiers.
- **Conflicts and adapters**: certain part pairs cannot coexist
  (Coastal gill + Mountain lung) without an **adapter part**
  (e.g., Tidal Bellows). Adapters are themselves harvested parts
  with their own lore and rarity.

### Parts catalog

- Each chapter unlocks ~15–20 new parts.
- Rarities: common / uncommon / rare / **named**.
- Named parts carry lore (the Mireling venom gland tells you who the
  Mireling was, why it was named, who first harvested one).

## Original IP

The Grafter's Guild, the Pure Strain Order, the bio-punk setting,
the biome taxonomy, every named creature (Mireling onward), every
named part, the 5-slot crafting structure, and the symbiosis +
adapter mechanic are original to Cleave Studios. The **build** verb
explicitly avoids Nintendo's creature-catching patents (see
`docs/IP-GUIDELINES.md`).

### Faction stances

- **Pure Strain Order** — religious-ecological preservationists.
  Creatures are sacred as their birth biomes made them; grafting
  destabilizes biome balance and produces beings with no rightful
  biome to return to. Aristocratic, well-funded, traditionalist.
- **Grafter's Guild** — working-class artisans and tinkerers. Life
  already self-modifies (parasitism, hybridization, symbiosis);
  grafting accelerates what nature does on its own. Egalitarian,
  craft-focused.

The player starts inside Pure Strain conviction and is forced into
Guild work. The campaign is the player working out which faction
holds more truth — or whether truth lives between them.

## Episodic plan

| Chapter | Biome (placeholder) | Teaches | Faction beat |
|---|---|---|---|
| 1 | The Mire (wetland) | Slots, basic harvest, first graft | PSO pursuit begins |
| 2 | Forge-mountains | First hybrid, heat-bearing parts | Guild internal politics |
| 3 | Whisperwood | Conflict-pairs + adapter parts | First PSO emissary; moral conversation |
| 4–6 | Escalating biomes | Adapter mastery; rare/named parts | Faction war intensifies |
| 7+ | Endgame biome | Compound parts; lineage reveal | Allegiance commitment |

Paid chapter expansions can ship new biomes with new parts catalogs
and new adapter rules.

## V-slice scope (Phase 3 target)

Per the original plan: **1 hub, 1 vignette, 1 battle, 4 starters,
1 graft event. ~30 min of polished play.**

- **Hub**: the Grafter's Guild workshop — one walkable room, the
  bench, the mentor figure, the parts catalog UI.
- **Vignette**: first harvest. Field encounter against a Mireling;
  defeating it produces a venom gland; the mentor walks the player
  back to the bench.
- **Battle**: 3v3 turn-based grid-row encounter against PSO scouts.
  Teaches front / back / flank positioning and innate-move
  triggering.
- **Starters**: four pre-built creatures across different biome
  leans — Mire-pure (heavy purebred bonus), Forge-pure, a mixed
  hybrid, and a creature with an unresolved conflict pair waiting
  for the player's first adapter decision.
- **Graft event**: the player slots the harvested Mireling venom
  gland onto a starter and refights the battle. The same battle
  plays differently with the new Toxic innate move — the V-slice's
  payoff moment.

Verification: ≥40% itch.io demo completion + ≥60% "would buy" signal
on the V-slice.

## Tone

**Layered**: *Atelier*-warm at the bench, soberly questioning in
the field. Workshop scenes lean cozy lighting, bench-craft
satisfaction, montage-friendly. Field and story scenes carry moral
weight — faction confrontations, the named lives behind named parts.
Sonically: warm acoustic at the workshop; sparser, darker tones in
the biome.

## Strategic role — marketing edge

Per the original plan, **every player's roster looks unique → natural
sharing/screenshot engine.** Implementation implications:

- Each crafted creature gets a **procedurally composed pixel-art
  sprite** that visibly shows which parts went where. Pixel-art
  discipline (per `docs/ART-BIBLE.md`) constrains the parts catalog
  to clean silhouettes.
- Players name their creatures; named-roster screenshots are
  shareable identity content.
- The bench UI itself is screenshot-friendly — a clean visual
  recipe.
- Procedural sprites mean a finite parts catalog produces a
  practically infinite content surface for sharing.

## Open questions for paper-prototype phase

- 5 slots vs. simpler (3–4) — where's the legibility ceiling for
  symbiosis bookkeeping?
- Procedural pixel-art sprite composition — how visually distinct
  can compositions feel while staying inside the 32×32 / 48×48
  discipline?
- Adapter-parts mechanic — does it add depth, or does it feel like
  artificial gating?
- Faction allegiance — does the renegade-protagonist arc need an
  explicit choice point, or does it stay narratively imposed
  throughout?
- Parts harvesting — does "I just killed a Mireling and now I'm
  taking its venom gland" stay ethically weighted across hundreds
  of harvests, or does it numb? What design countermeasures keep
  named creatures named?
