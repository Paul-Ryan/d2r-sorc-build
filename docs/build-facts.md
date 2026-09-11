# Settled facts and decisions

What the guide already rests on, and why. Read this before changing a number —
most of these were reasoned through once and shouldn't be re-derived.

The guide itself is the published version of all this; this file is the part
that's easy to lose: the *reasoning*, the constraints that aren't visible in the
final text, and the things deliberately left open.

## The build

Fire Ball → Frozen Orb hybrid Sorceress. Frozen Orb is the primary opener; Fire
Ball is the answer to cold-immune packs and single targets. Two elements
because Hell has immunes to each, and the merc's Infinity covers the rest.

## Budgets

These are the two hard constraints everything else is fitted into.

**Skill points — 110 by level 99.** 98 from leveling, 12 from quests: Den of
Evil, Radament's Lair, and The Fallen Angel (Izual), once per difficulty each.
Chosen because all three are low-risk quests almost every character finishes
anyway.

**Stat points — 505 by level 99.** 490 from leveling (5/level, 2→99) plus 15
from Lam Esen's Tome across three difficulties. Starting attributes are
str 10 / dex 25 / vit 10 / energy 35, on top of the 505.

Unlike skills, there is **no stat surplus**. Every point strength takes is life
not gained.

## Sorceress skill unlock levels (verified 2026-09-11, diablo2.io)

Reference data — check here before writing a level into the guide.

| Level | Skills this build touches |
| --- | --- |
| 1 | Fire Bolt, Warmth, **Frozen Armor**, Ice Bolt |
| 6 | Telekinesis, Static Field, Frost Nova, Ice Blast |
| 12 | Fire Ball |
| 18 | Teleport, **Glacial Spike** |
| 24 | **Blizzard**, Energy Shield |
| 30 | Frozen Orb, Cold Mastery, Fire Mastery |

Corrections this table produced:

- **Frozen Armor is level 1, not 6.** The old Phase 1 table had a whole row
  gating it at 6. Fixed.
- **Telekinesis unlocks at 6, not 12.** The old checkpoint claimed it "unlocks
  together" with Fire Ball at 12. It is a 1-point prerequisite tax due any time
  before Teleport at 18 — there is no reason to pay it at 12 specifically.
- Glacial Spike is 18 and Blizzard is 24 (both higher than commonly assumed),
  which is why the Phase 2 respec can't happen much before 30 anyway.

Prerequisite chains: Fire Bolt → Fire Ball. Telekinesis → Teleport. Ice Bolt →
Ice Blast → Glacial Spike → Blizzard → Frozen Orb (Frost Nova also required).
Cold Mastery and Fire Mastery have no prerequisites.

**Fire Mastery's curve is lopsided.** Level 1 gives **+30%**; every level after
gives **+7%**. (Level 20 totals +163%.) It is also **multiplicative** with
synergies, not additive — damage ≈ base × (1 + synergy) × (1 + mastery).

That makes the first Fire Mastery point the best single point in the fire tree
and every subsequent one among the worst. At level 30 with Fire Bolt at 1:

| Next point | Damage change |
| --- | --- |
| Fire Mastery, 1st | **+30%** |
| Fire Bolt (→2) | +12.3% |
| Fire Mastery, 2nd | +5.4% |

Hence the level-30 gate on the Phase 1 rail: exactly one point, then back to
Fire Bolt. Same shape as the Static Field argument.

### Fire damage model — CONFIRMED (Paul supplied sources, 2026-09-11)

    damage = base x (1 + synergy) x (1 + mastery)

- **Synergies** add together into the base-damage bonus. They count **hard
  skill points only** — `+skills` from gear, charms, buffs and shrines do
  **not** raise a synergy bonus.
- **Fire Mastery** is a *separate multiplier* applied after base + synergies.
  As a skill, its own level **does** scale with `+skills`.
- **Gear `+% fire damage`** (facets, Eschuta's) adds **additively into the
  Fire Mastery bucket**, not as a third multiplier — so it further dilutes the
  marginal value of mastery points.

**The asymmetry is the whole story.** `+skills` inflate mastery and do nothing
for synergies. One hard point in Fire Mastery activates it at level `1 + your
+skills`, capturing the entire stack at once (`+skills` cannot activate a skill
with zero hard points). Fire Bolt gets no such boost, ever.

| | +0 skills | +6 skills |
| --- | --- | --- |
| Fire Mastery, 1st hard point | +30% | **+72%** |
| Fire Mastery, 2nd point | 5.4% | 4.1% |
| Fire Bolt, any point | 12.3% (at 1) → 3.8% (at 19) | identical — unaffected |

Fire Bolt's curve crosses below mastery's second point at roughly **Fire Bolt
12** with no gear, **Fire Bolt 18** at +6 skills. More `+skills` therefore push
*harder* toward "one mastery point, then Fire Bolt".

### Cold Mastery — RESOLVED (mechanics supplied by Paul, 2026-09-11)

Curve: **−20% enemy cold resist at level 1, −5% per level after.** Linear — no
diminishing returns in the number itself, unlike Fire Mastery.

Three mechanics that matter more than the curve:

- A monster's cold resistance **floors at −100%**. With +6 skills, a hard Cold
  Mastery of ~11 already reaches it, so further points do *nothing* against a
  0%-resist monster and only help against ones carrying positive cold resist.
- Against a monster that is **already immune** (≥100%), every resistance debuff
  — Conviction, Lower Resist, Cold Mastery — applies at **1/5 strength**.
- **Cold Mastery cannot break an immunity at any level.** It only works once
  something else has.

**Verdict: Cold Mastery 10 / Fire Mastery 11 by default.** The five points
between rows 11 and 13 are near-even (≈+15% Frozen Orb vs ≈+17% Fire Ball), so
the tiebreak is an item: without a **Cold Rupture** sunder charm cold immunes
are Fire Ball's problem alone, so the points belong in Fire Mastery; with one,
Frozen Orb handles immunes and those Cold Mastery points pay ≈+21% there —
switch to Cold Mastery 15 / Fire Mastery 6. Reproduce with `cold.py`.

### CORRECTED — Infinity does not solve immunity

The guide claimed Conviction is "what actually makes Hell work" for cold- and
fire-immune packs. Overstated. At 1/5 effectiveness, level 12 Conviction's
−85% lands as ≈−17%, breaking immunities up to ~116% and nothing above. Many
Hell cold immunes sit higher.

The real answer is a **Cold Rupture sunder charm** (Terror Zones), which forces
immunes to 95% so Cold Mastery can work on them. Fixed in the Gear tab (new
gap-flag in Hell), the Mercenary tab's Infinity card, and the Beyond Hell
Terror Zones card, which now frames sunder charms as the fix rather than a bonus.

### RESOLVED — Phase 3 rewritten, Fire Bolt over Fire Mastery

Applied 2026-09-11 at Paul's direction. Model confirmed from sources he supplied.

Phase 3 spends **20 points on Fire Mastery 0→20** and leaves Fire Bolt at its
1-point prerequisite. At +6 skills, for the same budget:

| Fire budget | Optimal | Multiplier | Current shape | Gap |
| --- | --- | --- | --- | --- |
| 6 | Bolt 6 / Mast 1 | ×3.16 | ×2.36 | +34% |
| 11 | Bolt 11 / Mast 1 | ×4.37 | ×2.76 | +58% |
| 20 | **Bolt 19 / Mast 2** | **×6.55** | ×3.48 | **+88%** |
| 26 | Bolt 20 / Mast 7 | ×8.13 | ×6.04 | +35% |
| 31 | Bolt 20 / Mast 12 | ×9.46 | ×8.17 | +16% |

So the shape is **Fire Mastery 1 → Fire Bolt to ~19 → then more Fire Mastery**.
Near-corner, not the balanced mix an earlier version of this note claimed (that
version assumed synergies also scaled with `+skills`; they do not).

**Final Phase 3 allocation (72 points, closes to exactly 110):** Fire Ball
7→20 (13), Ice Bolt 1→20 (19), Fire Bolt 1→20 (19), Static Field 0→1 (1),
Cold Mastery 1→10-15 (9-14), Fire Mastery 0→6-11 (6-11).

The old 6–11 point surplus is gone — it was an artifact of over-funding Fire
Mastery, and Fire Bolt absorbs it. Static Field's single point is now an
explicit row; it was previously assumed but never allocated anywhere.

**Fill order after Fire Ball maxes:** Fire Mastery ×1 (best single point in the
build) → Ice Bolt (Frozen Orb is the opener) → Fire Bolt (before Hell immunes)
→ the rest of Fire Mastery last, since those points are the weakest in the plan
at ~4% each and nothing is gated behind them.

**Only skill question still open:** Cold Mastery 10 vs 15, trading directly
against Fire Mastery 11 vs 6. Worth ~+17% fire damage. Cold Mastery is harder
to price (it cuts *enemy* resistance, and overlaps with Infinity's Conviction)
and also scales with +skills. Deferred to the Monarch respec.

Reproduce with `fire2.py` (scratchpad) if the numbers need re-checking.

**Fire Bolt → Fire Ball is +14% per level.** Verified. The `+16%` figure that
turns up in search results is the *reverse* synergy (Fire Ball → Fire Bolt) and
does not apply to the open decision below.

## Phase 1 is a rail, not a schedule

Changed 2026-09-11 at Paul's direction. The old Phase 1 table scheduled points
by level range with running Spent / Earned / Bank columns. It was replaced by a
**gate rail**: three stages keyed to the only real unlock gates (1, 12, 18),
with order and counts inside each, and the budget arithmetic demoted to a
single "does this add up?" checkpoint.

Why, so this doesn't get reverted:

- The schedule encoded one projected playthrough. Any quest point, death, or
  party XP desynced it — and the guide's own checkpoint told readers to re-add
  a column by hand.
- Spent / Earned / Bank proves affordability, which you verify once. It was
  occupying the space where "what do I click next" belongs.
- Invented level rows gave wrong facts the same authority as right ones, which
  is how Frozen Armor sat at level 6 unnoticed.

The one real scheduling fact — **hold your level-11 point so Fire Ball starts
at 12** — is now a flagged step on the rail instead of a `1` in a Bank column.
It's also soft: a quest point arriving early makes the hold unnecessary.

## Skill plan — two builds, not three phases

Restructured 2026-09-11 at Paul's direction. The tab used to read Phase 1 / 2 / 3.
Phases 2 and 3 were never two plans: Phase 2's 38-point table was literally the
first 38 entries of Phase 3's fill order, truncated. The "Phase" label implied a
decision point that does not exist — the target allocation is identical either
side of it.

There are **two builds and one event**:

1. **The leveling build** (1→35) — disposable, refunded entirely at the respec.
   Presented as the gate rail.
2. **The respec at 35** — an event, not a phase. Akara, free once per difficulty.
3. **The real build** (35→99) — one ordered list of all 110 points, with a line
   marking where the 38-point respec budget runs out.

The fill order is the reusable artifact: **you walk it more than once**, because
the Monarch respec resets skills too and you re-enter the same list, stopping
wherever your level leaves you. That is the strongest argument for ordering over
scheduling here.

Final order: prereqs (5) → utilities (4) → Fire Bolt 1 → Frozen Orb 20 →
Cold Mastery 1 → Fire Ball 7 **[38, respec budget]** → Fire Ball 20 (13) →
Fire Mastery 1 → Static Field 1 → Ice Bolt 20 (19) → Cold Mastery 10 (9) →
Fire Bolt 20 (19) → Fire Mastery 11 (10). Totals exactly 110.

### Resolved: Ice Bolt before Fire Mastery

Both reach 20/20 by level 99 under either order, so there's no final-build
cost — only mid-game clear speed. Ice Bolt wins because it synergizes Frozen
Orb, which is the opener, and early points compound over the 35→70 stretch.

### Resolved: Static Field gets exactly one point

Damage is 25% of current life at *every* skill level. Points buy radius only,
~0.67 yd each. The plan already carries +5 to skills from Lore and two Spirits,
which runs a 1-point Static at roughly 8 yards for free.

Two limits that make it a boss tool, not an opener: it floors at 50% of monster
life in Hell (33% in Nightmare), and it's lightning damage, so it does nothing
to lightning immunes — **and Conviction from Infinity does not help**, because
resistance debuffs are ignored in Static Field's calculation.

### Still open: Fire Bolt

Fire Bolt is Fire Ball's synergy at +14% fire damage per level, and the plan
leaves it at the 1-point prerequisite. 1→20 costs 19 points (≈ +266%) — more
than the surplus. The surplus buys a lot of it, though: hold Cold Mastery at 10
and 11 points take Fire Bolt to 12 (≈ +154%); push Cold Mastery to 15 and 6
points take it to 7 (≈ +84%).

**Deliberately unresolved.** The Monarch respec reopens the whole skill tree
anyway, so it gets settled there. Don't close this out without a decision from
Paul.

## Stats

Strength to gear minimum, everything else to Vitality, dexterity and energy at
base. Blocking isn't worth it on a caster; Spirit, Stealth, and Warmth cover
mana better than energy points do.

**The Monarch is the whole stat problem.** The Hell off-hand Spirit needs a
4-socket Monarch: 156 strength, level 54. That's 146 points over base — about
29% of the lifetime budget, permanent once equipped. The plan is to carry only
what the sword needs (43 on Crystal, 48 on Broad), bank the rest in Vitality,
and **respec into the Monarch only once one is actually in hand**. Charms and
+all-stats gear (Annihilus, Hellfire Torch) claw back 20–40.

Monarch is the floor, not a preference — the lowest-strength 4-socket
non-class shield in the game. There is no cheaper base to look for.

## Respecs

Akara resets **stats and skills together**, free, **once per difficulty** —
three per character. Phase 2 spends one, the Monarch spends another, one spare.
Beyond that, a Token of Absolution (cube the four Hell act-boss Essences) is
unlimited.

The coupling is useful, not a limitation: the Monarch respec reopens the skill
tree at the same moment, which is why Fire Bolt is deferred to it.

## Gear

Seven runewords, farmed in this order — level requirement first, rune tier
second:

| # | Runeword | Slot | Lvl | Runes | Source tier |
| --- | --- | --- | --- | --- | --- |
| 1 | Stealth | armor | 17 | Tal + Eth | Normal Countess |
| 2 | Leaf | weapon (early) | 19 | Tir + Ral | Normal Countess |
| 3 | Ancients' Pledge | off-hand | 21 | Ral + Ort + Tal | Normal Countess + one Ort |
| 4 | Spirit (sword) | weapon | 25 | Tal + Thul + Ort + Amn | Nightmare Countess |
| 5 | Lore | helm | 27 | Ort + Sol | Nightmare Countess |
| 6 | Insight | merc weapon | 27 | Ral + Tir + Tal + Sol | Nightmare Countess |
| 7 | Spirit (shield) | off-hand | 25* | Tal + Thul + Ort + Amn | needs a Monarch |
| 8 | Infinity | merc weapon | 63 | Ber + Mal + Ber + Ist | Hell + Ber farming |

Stealth and Leaf are grouped because every rune they need drops from **Normal**
Countess. Spirit/Lore/Insight are grouped because Ort, Sol, Thul, and Amn all
drop together from **Nightmare** Countess — one farming stretch, not three.

`25*` on the shield Spirit is the runeword's level, not the gate — the Monarch
base is (level 54, 156 str).

**Ber is the real bottleneck.** Countess can't drop Ber at *any* difficulty,
and no boss reliably does. Hell Countess tops out at Ist, so she still covers
Infinity's Mal and one Ist. The two Bers come from Lower Kurast super chests,
Travincal, Cow Level, or Terror Zones — or trade, which is what most people do.

### Resolved: Ancients' Pledge holds the off-hand until the Monarch

Added 2026-09-11. The plan previously went from the Spirit sword (level 25)
straight to the Hell Monarch Spirit, leaving ~30 levels of undefined off-hand.

**Ancients' Pledge in a 3-socket Kite Shield.** Fixed stats, no rolls: fire
+48%, lightning +48%, poison +48%, cold +43%, +50% enhanced defense, 10% damage
goes to mana.

Why it wins, in order of weight:

- **Strength is nearly free.** Kite Shield is 47 str; the Spirit sword already
  needs 48 (Broad) or 43 (Crystal). So it costs 0 or 4 points — which is the
  whole game given the Monarch already wants 146.
- **It's the largest fire-resist item anywhere in the plan**, against the
  documented fire gap.
- **No new farming.** Ral and Tal are Normal Countess; the single Ort comes
  with Lore's.
- **Alternatives all trade resist for skills and lose.** Splendor (lvl 37,
  Eth+Lum, +1 skill / +10% FCR), Rhyme (lvl 29, Shael+Eth, +25 all resist /
  Cannot Be Frozen), Lidless Wall (unique Grim Shield, lvl 41, 58 str, +1 skill
  / 20% FCR). None beats 48% fire, and Stealth + one Spirit already clears the
  37% FCR breakpoint, so the skills/FCR they offer aren't what's scarce.

Base shopping: buy it **already socketed from Fara**, Act 2 Normal, resetting
stock at the waypoint. Kite Shield caps at 3 sockets, so there's no overshoot
trap like the Crystal Sword. **Do not spend a Larzuk charge** — all three are
committed. Large Shield is diablo2.io's suggested fallback base.

**Blocking is a decoy on every shield in this build.** Block chance is
`(blocking% × (dex − 15)) / (clvl × 2)`; at base 25 dex that's ~3%. Never pay
strength for a better-blocking base. Consistent with the existing skip-dex call.

### The Monarch swap is a net resist loss

Non-obvious and worth keeping: replacing Ancients' Pledge with the Hell Spirit
shield **lowers** your resists. Spirit's shield half has cold/lightning/poison
at 35% each and **no fire**. Net: −48 fire, −13 lightning, −13 poison, −8 cold,
in exchange for +2 skills, FCR, FHR, +22 vitality, ~+100 mana.

The trade is still correct — by Hell the skills and cast rate outweigh it — but
it means the fire gap gets *worse* at that moment, not better. Rings, amulet,
and charms have to absorb it.

### Checked: there is no cheap 4-socket shield

Kite Shield → Dragon Shield → **Monarch** are one upgrade family, so the
obvious hope is that a lower tier could hold Spirit. It can't: Kite Shield caps
at **3** sockets, and diablo2.io states Monarch has "the lowest strength
requirements of those which can have 4 sockets." The 156-strength respec stands.
Don't re-investigate this.

### Sockets — three Larzuk charges, four items that need four sockets

Larzuk sockets one item per difficulty, three for the character's life. The
plan needs 4-socket bases for the Spirit sword, the Monarch, and two merc
polearms. Resolution: **Larzuk gets the Spirit sword and the Monarch** (carried
longest); **cube the polearms**, since Insight is replaced by Infinity anyway.

Larzuk gives the *maximum* the base allows on white/gray, 1–2 on magic, exactly
1 on rare/set/unique. Always hand him white or gray.

**The Crystal Sword trap.** Broad Sword and Crystal Sword roll identical Spirit
stats, so take whichever drops first — Crystal is even 5 strength cheaper (43
vs. 48). But a **Broad Sword caps at 4 sockets always**, while a **Crystal
Sword above ilvl 40 maxes at six**, and a 6-socket sword can't hold Spirit. The
charge is then wasted and doesn't come back. So: Broad Sword → Larzuk, Crystal
Sword → Cube, unless you know the Crystal is ilvl 26–40.

Cube socket recipes work on **normal (white/gray) items only** and give a
**random** count from 1 to the base's max — retry freely, two runes and a
perfect gem per attempt. Note the shield recipe wants an Amn, the same rune
Spirit needs.

## Numbers

**FCR/FHR breakpoints** — see [sources.md](sources.md) for the convention
question. The guide's tables match d2runewizard exactly. Where the gear lands:

- Stealth (25%) + one Spirit (25–35%) = **50–60% FCR**, past the 37%
  breakpoint (20 frames), short of 63%.
- Second Spirit in Hell = **75–95%**, clears 63% (19 frames).
- 105% (18 frames) needs dedicated FCR from rings/amulet/gloves — a later
  target, not something to plan around.
- **FHR is free**: Stealth 25% + Spirit 55% = 80%, clearing the 60% breakpoint
  (8 frames). Both Spirits = 135%, past the final 86% breakpoint (7 frames).
  Never spend a slot on FHR. Corollary: dropping Spirit costs 55% FHR.

**Resist penalties** are flat per difficulty: Normal 0, Nightmare −40%,
Hell −100%. The 75% cap doesn't move, so raw resistance needed is 75 / 115 /
175%. Malah's Prison of Ice scroll gives +10% all resists per difficulty, +30%
across all three.

### The fire resistance gap — the guide's biggest open problem

Lore + Stealth + both Spirits + three Scrolls of Resistance lands roughly at
**fire 30%, cold 65%, lightning 95%, poison 95%** raw, against 175% needed.
Every element is short and **fire is the hole — not one item in the plan grants
a point of it.** Rings, amulet, and charms have to close about 145% of fire and
110% of cold.

Cold Mastery and Fire Mastery lower *enemy* resistance; they don't raise yours.
The Sorceress has no defensive resist skill.

Order of operations: **cap resists first, chase 105% FCR only after.** An
uncapped resist in Hell kills you; a missed cast breakpoint just makes you
slower.

## Mercenary

**Act 2 Offensive (Might), hired in Nightmare.** A merc's aura level and stats
lock in at the difficulty hired from — a Nightmare hire scales through Hell, a
Normal one doesn't. Offensive over Holy Freeze or Prayer because an item-granted
aura (Meditation, Conviction) runs *alongside* the merc's own class aura rather
than replacing it, so Might stacks with whatever the weapon grants.

The merc isn't a convenience. The Sorceress has no minion and no defensive
skill, so it's the build's only physical damage and its only aggro sink.

Weapon: Insight (Meditation — effectively infinite mana for *you*, not just the
merc) until Infinity (level 12 Conviction, up to −85% enemy resistance).

**Open gap:** merc survivability isn't planned anywhere. A naked merc dies on
repeat in Hell and stops contributing Might or Conviction exactly when it
matters. Vampire Gaze and Duriel's Shell or Treachery are the usual cheap
answers — this needs to become its own line item.

## Quests that must not be skipped

Once Leaf and Stealth are done it's fine to rush the rest of Normal, except:

- **The Horadric Cube** (Act 2, "The Horadric Staff") — every socket recipe and
  rune upgrade here needs it.
- **Larzuk / "Siege on Harrogath"** (early Act 5, kill Shenk) — this is what
  grants the socket charges the plan counts on, and it's easy to blow past.
- **The Golden Bird** (Act 2) — permanent +20 max life, once per difficulty.
- Deckard Cain isn't build-critical but is two minutes for free identifies.

Charsi's Imbue is safe to walk past.

## After Hell Baal

Terror Zones (hourly rotating, monsters to ~level 96 in Hell, and the source of
**Sundered Charms** — a cold-sundering charm opens packs Frozen Orb can't
touch) and the Hellfire Torch (Uber Tristram; +3 to a random class's skills,
+10–20 all attributes, **+10–20 all resistances** — a real answer to the fire
gap regardless of which class the skills land on).

Nothing past those is load-bearing. Level 99 is optional polish; XP costs
balloon and most players stop in the 90s by choice.
