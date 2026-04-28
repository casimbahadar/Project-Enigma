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
