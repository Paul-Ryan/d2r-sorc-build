# Working on this repo

Paul's Diablo II: Resurrected Sorceress build guide — a Fire Ball → Frozen Orb
hybrid. One hand-written HTML file, no build step, no dependencies, deployed to
GitHub Pages on every push to `main`.

Nearly every change here is **content**: a number, a verdict, a new section. The
CSS and the tab script are done and rarely need touching.

## Read these first

| Doc | When |
| --- | --- |
| [docs/build-facts.md](docs/build-facts.md) | Before changing any number, verdict, or plan step. It records what's already settled and *why*, so decisions don't get re-litigated. |
| [docs/sources.md](docs/sources.md) | Before looking a game fact up. It says which sites are actually fetchable, their URL patterns, and where sources disagree. |

Both are for the guide's *content*. The rest of this file is how the page is
built.

## Layout

`index.html` is one file in four parts: `<head>` (meta + Google Fonts link +
the entire stylesheet inline), the masthead, five tab panels, and a `<script>`
at the bottom holding the theme toggle and the tab controller.

Five tabs. Tab buttons and panels are in the same order; the README's layout
table happens to list them in a different one.

| Tab | Button id | Panel id | Hash |
| --- | --- | --- | --- |
| Skill Points | `tab-points` | `panel-points` | `#points` |
| Gear | `tab-gear` | `panel-gear` | `#gear` |
| Stats & Keys | `tab-stats` | `panel-stats` | `#stats` |
| Mercenary | `tab-merc` | `panel-merc` | `#merc` |
| Breakpoints & Resists | `tab-numbers` | `panel-numbers` | `#numbers` |

Adding a tab means four edits: a `<button class="tab">` with its two-digit
`<span class="idx">`, a `<section role="tabpanel" hidden>` (the first panel is
the only one without `hidden`), the README's layout table, and this one. The
script wires everything by `aria-controls`, so no JS change is needed.

## Component vocabulary

Reuse these rather than inventing markup — the page reads as one system because
every section is built from the same dozen pieces.

**Structure**
- `.section` → `.section-head` (an `<h2>` plus a `<span class="section-note">`
  right-aligned label) → content. One topic per `.section`.
- `.lede` — a muted intro paragraph under the head.
- `.split` — two columns above 940px: wide content left, a `.checkpoint` right.
  Below that it stacks.
- `.bp-cols` — equal-width auto-fit columns, for two tables side by side.

**Prose callouts**
- `.checkpoint` — bordered aside with a small caps `<span class="mark">` label
  and one `<p>`. This is where the guide's reasoning lives.
- `.checkpoint.gap-flag` — the same, in warning red. Reserved for genuine holes
  in the plan and traps (an unrecoverable quest charge, a resist the build
  never covers). Don't spend it on ordinary emphasis.
- `.verdict` — a resolved question: `.q` (the question), `.a` (the answer, with
  `<b>` fire-colored or `<b class="cold-b">` cold-colored), then `<ul
  class="reasoning">` of `<li>`s each opening with a bolded claim.

**The skill-point rail** — Phase 1's layout, and the model to reach for when
order matters more than schedule.
- `.railstage` — one stage: a `.railhead` (`.lvl` gate label + `.unlock`
  description) over a `.railbody` of `.spendrow`s.
- `.spendrow` — three columns: `.sk` (skill), `.amt` (how much), `.why`
  (reasoning). Add `.sink` to the row that takes *every* point at that stage.
  Collapses to one column under 640px.
- `.railjoin` — the connector between stages; may be empty, or hold a
  `.joinnote`. Add `.flag` to turn it gold for a step that needs action
  (currently just the level-11 hold).

Gates in `.lvl` must be **real game unlock levels**, never planning estimates.
The old Phase 1 table invented level rows and hid a wrong one (Frozen Armor at
6; it's a level-1 skill) for who knows how long. See docs/build-facts.md for
the verified table.

**Cards and tiles**
- `.rwgrid` → `.rwcard` — one runeword. `.rwhead` (`.rwname` + `.rwlvl`),
  `.rwrunes` (the rune string and base), an optional `.rwstats` block, then
  `.rwrow`s of `<b>Why</b>` / `<b>Where</b>` + `<span>`.
- Inside `.rwstats`: `.rwstats-label` header, then one `.rwstat` per line.
  Add `.roll` plus a `<span class="rolltag">rolled once</span>` for stats
  randomized at creation; use `<span class="hittag">per hit</span>` or
  `scales w/ level` for ordinary per-swing variance. The distinction matters —
  "rolled once" is the guide's signal that remaking the item is the only fix.
- `.tiles` → `.tile` with `.num` + `.label`, optional `.accent-fire` /
  `.accent-cold` top rule. For headline totals.
- `.statgrid` → `.statcard` (`.skip` variant for stats to ignore).
- `.padgrid` → `.padkey` (`.util` for triggers, `.off` for unbound).

**Tables** — always wrap in `.tblwrap`. Cells: `.num` right-aligns,
`.skill` is the wide descriptive column. `<span class="tag fire">` /
`<span class="tag cold">` are inline chips. `.mono` for figures in running prose.

Two row highlights, and the difference matters:
- `<tr class="row-mark">` — tints the row. Use this for grouping, a
  recommended option, or the case that matters most. This is the default.
- `<tr class="bp-hit">` — the same tint **plus a literal "reached" label**
  stamped on the first cell by CSS. Only for a threshold the build genuinely
  lands on, in a table listing thresholds it might not. There are exactly two
  in the page (37% FCR, and Static Field's ~8 yd radius); if you're reaching
  for a third, you almost certainly want `row-mark`.

## Conventions

- **HTML entities, not literal characters.** The file uses `&mdash;`, `&ndash;`,
  `&times;`, `&rarr;`, `&minus;`, `&hellip;` throughout. Match it.
- **Elements are color-coded.** Fire is `var(--fire)`, cold is `var(--cold)`,
  gold is for randomized rolls and UI accents. Never hardcode a hex.
- **The dark palette is defined twice** — once under
  `@media (prefers-color-scheme: dark)` and once under `:root[data-theme=dark]`,
  with identical values. Change a token and you change both blocks.
- **Voice.** Second person, present tense. Every claim carries its reason in the
  same breath, and the guide says plainly when something is unresolved or a bad
  idea. It's a reference someone plays from, not marketing copy — no hype, no
  "pro tip".
- **Numbers get shown, not asserted.** If the plan says a phase costs 31 points,
  a table nearby adds up to 31.

## Checks before committing

There are no tests. Do this by hand:

```
python3 -m http.server 4173   # then open http://localhost:4173
```

- Click all five tabs; confirm the hash updates and a direct `#gear` load opens
  the right one.
- Toggle the theme both ways.
- Narrow the window under 640px.
- If a number changed, re-check the totals that depend on it — the skill ledger,
  the stat budget, and the resist math all cross-reference each other.
