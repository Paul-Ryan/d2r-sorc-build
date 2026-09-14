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

## Prerequisites (tab added 2026-09-12)

Verified facts behind the tab:

- **Expansion, not Classic.** Runewords were introduced in Lord of Destruction
  and cannot be made on a Classic character at all — which would void the entire
  Gear tab. Classic also has no Act 5, so no Larzuk socket quest. D2R ships both;
  the choice is a prompt at character creation and is permanent.
- **Online, not Offline.** The two are stored separately and **cannot be
  transferred in either direction**. Offline = no ladder, no trading, no
  cross-progression, no server backup. Decisive here because the plan needs two
  Ber runes (three with Chains of Honor) and the Gear tab's own math rules out
  farming or cubing them — trading is the only route, and offline has no one to
  trade with.
- **Battle.net account is free** — it is an account, not a subscription. The
  paid tier on Xbox is Microsoft's own online service, now sold as **Game Pass
  Essential / Premium / Ultimate** (replaced Xbox Live Gold). PS Plus on
  PlayStation.
- **Reign of the Warlock is not required.** Terror Zones and Sunder Charms both
  arrived in base D2R patches.
- **"Single Player" on the menu means offline.** What the guide recommends is an
  *online* character in a *private, empty* game — the terminology trips people.
  Monster life scales with player count, so solo is the easiest version of every
  fight.
- **Current ladder season** for the fresh economy — runes circulate; non-ladder
  Ber holders have held them for years. Characters roll to non-ladder at season
  end, nothing is lost.

## Trading on Xbox — verified 2026-09-14

Added as its own Prerequisites section. The tab previously said "open a public
game when you specifically want to trade" and never explained the rest, while
the entire Gear plan rests on trading for three Bers, a Shako, a Vipermagi and a
Kira's. That line now recommends a password game and points at the new section.

- **Cross-progression, not crossplay.** Constantly confused. Cross-progression =
  the same Battle.net character on every platform you own the game on. Crossplay
  = playing in a session with another platform, and D2R **does not have it**. So
  **Xbox trades with Xbox only.** This is the fact that makes the Ber hunt worth
  starting early — the pool is smaller and slower than PC's.
- **Console has a real lobby since patch 2.4.3.** Party Finder was replaced by
  **Game Creator** (public game, preset or custom name, optional **password**)
  and **Game List** (up to 40 games, filter by difficulty/ping, search by name).
  Plus **Private** for invite-only. So the "console has no lobby" claim that
  still circulates is out of date.
- **But there is still no text chat on console.** This is the actual answer to
  "how do you trade" — the lobby gets two people into a room; the negotiation
  has to happen on a trading board plus Xbox party voice chat. Nothing about a
  price can be settled in-game.
- **Where Xbox players post:** diablo2.io's trade browser has an Xbox platform
  filter (convenient — it's already the guide's primary source); d2jsp has a
  dedicated *D2:R Xbox Ladder Trading* forum and carries most serious high-rune
  trade; D2R Marketplace, the Xbox trading subreddit, and per-console Discords
  for the rest. Mode must match exactly: online, ladder, softcore, Expansion.
- **Known console bug:** closing the trade window while the other party is
  mid-drag **drops the item on the ground**, grabbable by anyone in the game.
  Combined with the ordinary last-second-swap scam, this is why a password game
  with one stranger beats a public game with five.
- **The PC escape hatch.** Owning D2R on PC too means the *same character* logs
  in there, so you can trade into the much larger PC pool and carry the items
  back to Xbox. Costs a second copy of the game. For the Ber hunt this is the
  single biggest lever available and belongs in the plan, not in a footnote.

## Quest rewards — verified 2026-09-12

| Quest | Act | Reward, per difficulty |
| --- | --- | --- |
| Den of Evil | 1 | +1 skill point |
| Radament's Lair | 2 | +1 skill point, **as a Book of Skill item** |
| The Fallen Angel (Izual) | 4 | **+2** skill points |
| Lam Esen's Tome | 3 | +5 stat points |
| The Golden Bird | **3** | +20 maximum life |

4 skill points per difficulty × 3 = the 12 the plan assumes.

Two corrections this produced:

- **The Golden Bird is Act 3, not Act 2.** The Gear tab said Act 2.
- **Radament's point does not auto-credit.** He drops a Book of Skill that must
  be picked up and *used* from inventory. Den of Evil and Izual credit on
  completion; Radament does not. Three difficulties = three books. This is the
  most-missed skill point in the plan and now has its own flag.

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

### Cubing runes up (added 2026-09-12)

Recipes: **3-to-1** from El through Pul (no gem below Amn; chipped gem from Amn,
flawed from Lum), then **2-to-1** from Um upward (flawed gem for Um, standard
from Mal, flawless from Sur). Gems are never the bottleneck — chipped gems drop
everywhere and upgrade 3-to-1 themselves.

Priced in Ral (Normal Countess's ceiling): **Ort 3, Thul 9, Amn 27, Sol 81.**
The practical cutoff is around Thul — above it, a Nightmare Countess run is
faster than the stack.

**The one that changed the plan: Ancients' Pledge is now fully Normal-farmable.**
Its only above-Ral rune is the Ort, which is 3 Rals in the Cube. Previously the
guide sent you to Nightmare Countess for it. Now you can wear it from level 21
through the whole Nightmare stretch, which is exactly when its resists matter.

**It does not solve Ber.** Hell Countess tops out at Ist; Ist→Gul→Vex→Ohm→Lo→
Sur→Ber is **64 Ist per Ber**, so **128 Ist** for Infinity's two. Cubing sets the
Ist/Ber exchange rate that trades are quoted in, but is not an acquisition plan.
Confirms the existing "trade for Ber" advice rather than replacing it.

**Unverified:** whether any of the high-rune recipes are ladder-only. diablo2.io
does not flag a restriction. It changes no advice here either way, since the Ber
math is hopeless regardless — but check before relying on it for anything else.

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

### Armor and helm past the runewords — verified 2026-09-14

The runeword list stops at Stealth (armor) and Lore (helm), and neither grants a
point of fire resistance. Since the fire gap is the guide's biggest open
problem, these two slots are the largest corrections available to it. Two new
Gear-tab sections cover them. All stats below fetched from diablo2.io.

**Where the "fire 30%" baseline comes from**, worked out explicitly so it can be
re-derived: Lore 30 lightning + Stealth 30 poison + Spirit shield 35
cold/lightning/poison + three Scrolls of Resistance 30 all. Fire is carried by
the scrolls alone. Matches the figure the guide already published.

#### Armor candidates

| Item | Lvl | Str | Key stats |
| --- | --- | --- | --- |
| Skin of the Vipermagi (unique Serpentskin Armor) | 29 | 43 | +1 all skills, 30% FCR, All Res +20–35, MDR 9–13, +120% ED |
| Smoke (Nef + Lum, 2os body) | 37 | base | **All Res +50**, 20% FHR, +75% ED, +280 def vs missile, +10 energy, lvl 6 Weaken charges, −1 light radius |
| Chains of Honor (Dol + Um + Ber + Ist, 4os body) | 63 | base | **+2 all skills, All Res +65**, +20 str, DR 8%, +70% ED, +200% dmg demons, +100% undead, 8% LL, replenish 7, 25% MF |
| Enigma (Jah + Ith + Ber, **3**os body) | 65 | base | +2 all skills, +1 Teleport, **+0.75 str/level**, +45% FRW, +750–775 def, +5% max life, DR 8%, +14 life/kill, 15% dmg to mana, +1% MF/level |
| Ormus' Robes (unique Dusk Shroud) | 75 | 77 | 20% FCR, +10–15% fire **and** cold **and** lightning skill damage, +3 random Sorc skill, regen mana 10–15% |

**Verdict: Vipermagi when one turns up, Smoke if resists are the problem, Chains
of Honor at the end.**

- **Vipermagi strictly beats Stealth here.** 43 strength is exactly a Crystal
  Sword's requirement, so on that base it costs zero stat points. More FCR than
  Stealth (30 vs 25), +1 skill, and the first fire resist in the build.
- **The FHR loss is one frame and temporary.** Stealth+Spirit = 80% (8 frames);
  Vipermagi+Spirit = 55%, still clearing the 42% breakpoint at 9 frames. Both
  Spirits = 110%, past 86%, and the gap closes entirely.
- **Smoke is the only schedulable one.** Nef is Normal Countess; **Lum is 3 Io in
  the Cube and Nightmare Countess tops out at Io** (verified — her special rune
  drop caps at Ral / Io / Ist by difficulty). So it falls out of the existing
  Spirit/Lore/Insight farming stretch. +50 all res beats Ancients' Pledge's 48
  fire.
- **Smoke's cost is the 37% FCR breakpoint.** No FCR at all, so Smoke + one
  Spirit = 25–35%, back to 21 frames. Honest trade, stated in the guide.
- **Chains of Honor costs a third Ber.** The plan already commits to trading for
  two (Infinity). This makes it three. Flagged in the Infinity farming note too.

**Enigma is a stat-budget item, not a resist item.** +0.75 str/level = +63 at 85,
+74 at 99, against the Monarch's 156 — cutting the 146-point bill to ~83 at
level 85, ~72 at 99. But
price the returned points honestly: **Sorceress gets 2 life per Vitality point**,
so 63 points back is ~126 life, not the several hundred it looks like at a
glance. The real draw is Teleport in the armor slot (which also refunds the
Telekinesis + Teleport skill points) and skipping a respec. Costs Jah + Ber, so
dearer than CoH while capping nothing. Second priority at best.

**Ormus' pays the two elements unequally,** and this follows from the fire model
already recorded above. Gear fire% adds *into* the Fire Mastery bucket; at Fire
Mastery 11 with +6 skills that bucket is ≈+142%, so a +15% line is worth ≈**+6%**
real damage. Cold has no damage-mastery bucket at all (Cold Mastery cuts *enemy*
resistance), so **+15% cold skill damage is a clean +15% on Frozen Orb**. Ormus'
is a Frozen Orb item that happens to mention fire. Carries zero resistance.

Its +3 skill roll **can** land on Fire Ball but **never** on Frozen Orb, Fire
Mastery, Cold Mastery, Hydra, or Lightning Mastery — those five are excluded.

#### Helm candidates

| Item | Lvl | Str | Key stats |
| --- | --- | --- | --- |
| Harlequin Crest (unique Shako) | 62 | 50 | **+2 all skills**, +1.5 life & mana per level (≈148 each at 99), **DR 10%**, +2 all attributes, 50% MF, **max 1 socket** |
| Nightwing's Veil (unique Spired Helm) | 67 | 96 | +2 all skills, **+8–15% cold skill damage**, +10–20 dex, +5–9 cold absorb, +90–120% ED, half freeze, Requirements −50%, **0 sockets** |
| Kira's Guardian (unique Tiara) | 77 | negligible | **All Res +50–70**, 20% FHR, Cannot Be Frozen, +50–120 def |

**Verdict: Harlequin Crest by default; Kira's Guardian if fire is still what
ends runs.**

- **Correction worth recording: Nightwing's Veil does NOT carry −enemy cold
  resistance.** That is a widespread misremembering (including in the first
  draft of this analysis). Its offensive line is +8–15% cold skill damage and
  nothing else. Verified on diablo2.io.
- **Shako beats Nightwing's for a hybrid.** Matches the +2 skills, then adds
  ~148 life, ~148 mana, 10% flat DR, and a socket, for 50 str instead of 96.
  Nightwing's only pays the cold half — and Fire Ball is what you switch to on
  cold immunes, exactly where the helm would contribute nothing.
- **The pairing arithmetic.** Dropping Lore + Stealth for **Chains of Honor +
  Kira's Guardian**, with the Spirit shield and three scrolls: fire **145–165**
  (Kira's roll), everything else comfortably over the 175 cap — against fire 30
  today. And it is net **+1 skill** versus Lore + Stealth, since CoH's +2
  replaces Lore's +1.
- **Shako + Um + CoH lands fire at ~110 — still 65 short.** Worth publishing:
  even the premium pairing does not cap fire alone. (Um in helm/armor = +15 all
  res; Um in shield = +22. Verified.)

**Trap: Andariel's Visage.** +2 all skills, +25–30 str, 8–10% LL, +70% poison
res — and **Fire Resist −30%**, against a build already 145% short on fire. The
standard fix (30% fire-res jewel) only breaks even and burns a Larzuk charge,
since Cube socket recipes are white/gray only. Skip on the Sorceress; it stays
an excellent *merc* helm.

**Also checked and passed over:** Tal Rasha's Guardianship (lvl 71, 84 str, 40
fire/cold/light res, 88% MF, Requirements −60%) — fine, but no skills and no
FCR, so Vipermagi beats it for this build unless you're building the Tal's trio
for magic find, which is a different plan.

### The Cube — consolidated into its own section 2026-09-14

Paul asked whether crafting deserved a tab. **Answer was no, and the section
that got built is broader than crafting**, because the real finding was that the
Cube was load-bearing in six scattered places with nothing tying them together —
and two of those six were not on the page at all.

The six jobs: upgrade runes, add sockets, upgrade gems, craft an amulet,
**Token of Absolution**, Hellfire Torch. The middle two were the gaps.

**Crafting is NOT important to this build, and the section says so.** Four
families: Blood (perfect ruby, physical builds), Hit Power (perfect sapphire,
melee), Safety (perfect emerald, defense/DR — irrelevant once armor/helm/boots
cap resists), Caster (perfect amethyst). Only Caster applies, and **only two of
its four recipes are worth the runes**:

| Caster craft | Base | Rune | Guaranteed | Verdict |
| --- | --- | --- | --- | --- |
| Amulet | any amulet | Ral | mana regen, +10–20 mana, **5–10% FCR** | **Yes** |
| Belt | Light Belt | Ith | same, **5–10% FCR** | Yes, unless Arachnid Mesh |
| Ring | any ring | Amn | mana regen, mana, +1–5 energy | **No** — no FCR, rare beats it |
| Gloves | Leather Gloves | Ort | mana regen, mana, +1–3 mana/kill | **No** — no FCR, Magefist beats it |

All four also take a jewel and a perfect amethyst; base must be **magic** quality.

The one genuinely notable property: **the crafted caster amulet is the only item
in the entire plan you can manufacture rather than wait for.** Everything else on
the upgrade track is a drop or a trade.

**Token of Absolution — added to the page, was only in this file.** Cube the four
Hell act-boss essences: Twisted Essence of Suffering (Andariel **and** Duriel),
Charged Essence of Hatred (Mephisto), Burning Essence of Terror (Diablo),
Festering Essence of Destruction (Baal). Right-click to reset skills and stats
fully, **no limit on how many you use**. This materially changes how the Monarch
respec reads — the "one spare" Akara charge is the last *free* reset, not the
last one. Cross-referenced from Stats & Keys.

**Walk past the unique upgrade recipes.** Exceptional/elite upgrades buy defense
(useless to a caster) and raise the strength requirement (unaffordable against
the Monarch's 146-point debt). Vipermagi upgraded wants 84 str instead of 43.

**Placement:** before *Cubing runes up*, so the overview precedes the two
existing deep-dive sections rather than trailing them. The crafting checkpoint
in *The six small slots* was trimmed to a pointer so the recipes live in one
place.

#### The six small slots — verified 2026-09-14

Amulet, two rings, gloves, belt, boots. The guide named them repeatedly and never
said what goes in them. Two new Gear sections now do.

**Max faster cast rate per slot** (this is the useful reference):

| Slot | Max FCR | Notes |
| --- | --- | --- |
| Amulet | **20%** | crafted caster: 5–10% preset + 10% *of the Apprentice* suffix. Highest of any amulet in the game. |
| Ring ×2 | 10% each | suffix only; caster craft does **not** give FCR on rings |
| Gloves | 20% | Magefist or Trang-Oul's Claws — the only two gloves with it |
| Belt | 20% | Arachnid Mesh only; crafted caster belt is 5–10% |
| Boots | none | — |

**Caster cube recipes** (magic base + jewel + perfect amethyst + rune): amulet
**Ral**, ring **Amn**, belt **Ith** (Light Belt base), gloves **Ort**. All four
guarantee mana regen + flat mana; **only the amulet and belt also guarantee
FCR**. This is the controllable route versus waiting on unique drops.

#### The fire gap closes — in the boots slot

The headline finding. Chains of Honor (+65) + Kira's Guardian (+50–70) + three
scrolls = **fire 145–165** against 175. **Aldur's Advance carries Fire Resist
+40–50%**, taking it to **185–215 — capped**. Cold/lightning/poison sit at
180–200 on the same set because the Spirit shield covers all three at 35.

**Three items cap every resist in the game**, which frees amulet, both rings,
gloves and belt to be pure cast rate. Stated honestly in the guide: substituting
a Harlequin Crest for Kira's leaves fire near 160 even with the boots, so that
variant still needs a ring or the amulet for the last stretch.

Aldur's is 95 strength — steep before the Monarch respec, free after it.

#### Named items, with the verdicts

| Item | Lvl | Str | Key stats |
| --- | --- | --- | --- |
| Magefist (Light Gauntlets) | 23 | 45 | **+1 Fire Skills, +20% FCR**, regen mana 25%, 1–6 fire dmg, +20–30% ED |
| Aldur's Advance (Battle Boots) | 45 | 95 | **Fire Resist +40–50%**, +40% FRW, +50 life, +180 stamina, 10% dmg to mana, indestructible |
| Arachnid Mesh (Spiderweb Sash) | 80 | 50 | **+1 all skills, +20% FCR**, slows 10%, +5% max mana, lvl 3 Venom |
| Mara's Kaleidoscope (amulet) | 67 | — | +2 all skills, All Res +20–30, +5 all attributes |
| The Stone of Jordan (ring) | 29 | — | +1 all skills, +25% max mana, +20 mana, 1–12 lightning |
| Raven Frost (ring) | 45 | — | Cannot Be Frozen, +15–20 dex, cold absorb 20%, +40 mana, +150–250 AR |

- **Magefist and Aldur's are the only two that aren't optional**, and both are
  cheap. Magefist's +1 Fire Skills matters more than it reads — per the fire
  model above, `+skills` raise Fire Mastery's *level*, and Fire Mastery is a
  multiplier on everything Fire Ball does.
- **Rings want rares, not uniques.** SoJ has no resist and no FCR; Raven Frost's
  Cannot Be Frozen **duplicates Kira's Guardian**. A boring rare with 10% FCR and
  a resist line beats both for what this build needs.
- **The crafted caster amulet beats Mara's only from character level 93.**
  Corrected 2026-09-14, same day it was first written. **+2 class skills is an
  affix-level-90 roll**, and a craft's item level is `floor(clvl/2) +
  floor(ilvl/2)` — so at clvl 93 with a gambled base you land exactly on 90 and
  the affix becomes reachable. Below 93 it effectively cannot appear, and the
  craft gives cast rate and mana without the skills. **Mara's is the better
  amulet for most of the game.** The FCR value of the craft is real at any
  level, though: the preset plus *of the Apprentice* (alvl 5, +10% FCR, trivially
  common) is up to 20%, which no rare or unique amulet can match.
  Sources word the preset differently — d2runewizard says 5–10% FCR,
  diablo2.io says 10%. The guide uses 5–10%; the "up to 20%" total holds
  either way.
- **Arachnid Mesh cannot drop below monster level 87** (one of only three items
  with qlvl 87, alongside Tyrael's Might and Azurewrath), which rules out the
  usual farming targets. Treat as a trade; crafted caster belt is the makeable
  version.

**Belt potion rows** (Arreat Summit, authoritative): Sash 8, Light Belt 8, Belt
12, Heavy Belt 12, Plated Belt 16. **All exceptional and elite belts have 16**
regardless of base, so it stops mattering once you're in real gear.

Magefist (23) and Aldur's Advance (45) were added to the Gear tab's upgrade
table, since they're as load-bearing as Vipermagi and Smoke. The other four
small-slot items stayed in their own section — the table is about priorities,
and they aren't priorities.

#### Two farming tables, not one (added 2026-09-14)

The armor/helm upgrades are listed in the Gear tab's "Farming order" section, in
a **second table** below the runeword one rather than merged into it. The
runeword table has a property worth protecting: it is a list you can *finish*,
because every rune in it is reachable by deciding to go and get it. Merging
eight uniques and optional runewords into it would quietly destroy that.

Second table is ordered by required level (not priority), and carries two chips:

- `.tag.cold` **make** — Smoke, Chains of Honor, Enigma. Behaves like the first
  table.
- `.tag.luck` **find** — the five uniques. New CSS class, gold, reusing the
  meaning gold already carries on `.rolltag`: not in your control. You cannot
  farm a named unique into existence the way you can farm a rune.

`row-mark` tints the five actually recommended (Vipermagi, Smoke, Harlequin
Crest, Chains of Honor, Kira's Guardian). The three untinted rows — Enigma,
Nightwing's Veil, Ormus' Robes — are real but answer something other than the
resist gap, and the checkpoint under the table says which.

#### Larzuk arithmetic was wrong in the guide

The Ancients' Pledge checkpoint said "all three are already committed to the
Spirit sword and the Monarch" — three charges, two items. Corrected. **Two are
committed; the third is the reserve** for a polearm the Cube won't roll. If the
Cube cooperates, the **Harlequin Crest has the strongest claim on the spare**,
because it is the only item here that cannot be socketed any other way.


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

### The fire resistance gap — RESOLVED 2026-09-14

**Was the guide's biggest open problem. It is now closed, and the reasoning is
above** (see *Armor and helm past the runewords* and *The fire gap closes — in
the boots slot*). Kept here because the framing recurs.

The problem: Lore + Stealth + both Spirits + three Scrolls lands roughly at
**fire 30%, cold 65%, lightning 95%, poison 95%** raw, against 175% needed.
Fire is the hole — **no runeword in the core plan grants a point of it.**

The answer is three items, not "rings, amulet and charms": **Chains of Honor
(+65), Kira's Guardian (+50–70), Aldur's Advance (fire +40–50)** puts fire at
185–215 and everything else at 180–200. The small slots are then a cast-rate
problem, not a resist one.

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

### Merc survivability — RESOLVED 2026-09-14

Was the tab's open gap; now three sections (Why he dies / Mercenary helm /
Mercenary armor). All stats verified on diablo2.io.

**The finding that drives everything: neither merc weapon carries life steal.**
Insight has none, Infinity has none, and the Act 2 merc has no innate leech. So
from level 27 to the end of the game he has no in-combat healing at all unless
the helm supplies it. That reframes the helm slot from "nice defensive item" to
"the only sustain in his kit", and it is why he dies.

Three supporting mechanics, all verified:

- **The merc eats the same −100% Hell resist penalty** players do, with no
  scrolls, no charms and four fewer slots. Two items carry his whole resist
  total — hence a resist armor over a damage one.
- **Leech is a percentage of damage dealt**, so his offensive stats are
  defensive stats. Attack speed compounds it (leech is per hit, not per second).
  This is the argument for Treachery's +45% IAS, and why Fortitude is genuinely
  a survivability item.
- **Ethereal items do not lose durability on a mercenary.** Free +50% defense
  and −10 to strength/dex requirements. Always build merc gear in eth bases.
- **Mercs are NOT exempt from strength/level requirements** (commonly assumed).
  Act 2 merc gains ~1.5 str/level, which is what makes Crown of Thieves (103
  str) and Andariel's (102 str, level 83) genuinely late items.

#### Helm — verdict: Vampire Gaze at 41, stop there

| Item | Lvl | Str | Key stats |
| --- | --- | --- | --- |
| Vampire Gaze (Grim Helm) | 41 | 58 | 6–8% LL, 6–8% ML, **DR 15–20%**, MDR 10–15, +100% ED, 6–22 cold dmg, 15% slower stamina |
| Crown of Thieves (Grand Crown) | 49 | 103 | **9–12% LL**, +33 fire res, +50 life, +25 dex, +35 mana, +160–200% ED, 80–100% gold |
| Tal Rasha's Horadric Crest (Death Mask) | 66 | 55 | **10% LL**, 10% ML, All Res +15, +60 life, +30 mana, +45 def |
| Andariel's Visage (Demonhead) | 83 | 102 | +2 skills, 20% IAS, 8–10% LL, +25–30 str, +70 psn res, **−30 fire res**, 1 socket |

Leech is near-identical across three of them (8 / 10 / 9–12%) — not the
difference between living and dying. **Damage reduction is**, and Vampire Gaze
is the only one with it. It also arrives far earlier than the rest. Tal's Crest
is the sidegrade if he's dying to elemental rather than physical (and it's cheap
because it's the Tal's piece Sorceresses discard). Andariel's is the only true
upgrade; socket a 30% fire-res jewel and the penalty cancels.

Note the **deliberate asymmetry with the Gear tab**: Andariel's is a trap on the
player's head and correct on the merc's, because he can erase the fire penalty
with the helm's own socket and the player's Larzuk charges are already spent.

#### Armor — verdict: Smoke at 37, Treachery at 43, stop

| Item | Lvl | Cost | Key stats |
| --- | --- | --- | --- |
| Smoke (Nef + Lum, 2os) | 37 | Normal Countess + 3 Io | All Res +50, 20% FHR, +75% ED, +280 def vs missile |
| Duriel's Shell (Cuirass) | 41 | 65 str | +50 cold / +20 fire,lt,psn res, CBF, +15 str, +1 life/level, +160–200% ED |
| Treachery (Shael + Thul + Lem, 3os) | 43 | NM + Hell Countess | **5% CtC lvl 15 Fade when struck**, 25% CtC Venom, +45% IAS, +20% FHR, +30 cold res |
| Fortitude (El + Sol + Dol + Lo, 4os) | 59 | **needs a Lo** | +300% ED, +200% ED def, All Res +25–30, +5% max lt res, life/level, DR 7 |

**Level 15 Fade = +60% all resistances and 15% physical damage reduction for 288
seconds.** Verified. Nearly five minutes from one trigger, on a character who
gets struck constantly — so it's up permanently in practice. That is a larger
survivability number than Fortitude's +25–30 resist, and it arrives 16 levels
earlier.

**Fortitude loses on rune economy, not on stats.** It needs a **Lo**, which is
above Hell Countess's Ist ceiling and therefore a trade — competing directly
with the three Bers this plan already owes (Infinity ×2, Chains of Honor ×1).
Treachery's runes are Shael/Thul (Nightmare Countess) and **Lem, which is inside
Hell Countess's range**. No new farming route. Fortitude stays correct if a Lo
ever turns up; it is just behind Infinity and both of the player's armors in
trade priority.

**The two slots are designed to interlock** and the guide says so: Treachery's
+45% IAS multiplies whatever leech the helm gives, and Fade's physical mitigation
stacks with Vampire Gaze's. Helm heals him, armor reduces what he needs healed.

## Full-guide review — 2026-09-14

Paul asked for a cleanup pass after a session that roughly doubled the page.
What it actually found:

**A real structural bug.** The Gear tab was missing one `</div>` — *The helm
slot* never closed, so *The six small slots* and *Beyond Hell* were nested
inside it. **This was invisible to both of the checks being used**: whole-file
div counts balanced (the closer existed, just in the wrong place), and an
HTML-nesting parser reported clean (the tree was well-formed, just wrongly
shaped). It was only caught by tracking nesting *depth at each section opener*.
Added to the AGENTS.md checklist; it is the check that matters after inserting
a section by line number.

**Redundancy removed** (all introduced the same day the content was written):

- **Smoke's full stat block appeared twice**, in the Gear armor section and the
  Mercenary armor section — two copies of the same numbers to keep in sync. The
  merc copy is now a pointer, matching what Insight and Infinity already did.
- **The "fire 30%" arithmetic appeared four times**, and the "three items cap
  everything" resolution three times. Kept one canonical statement of each (the
  armor-slot breakdown and the small-slots resolution). The Hell-section flag
  and the Breakpoints flag are now pointers.
- **The "rolled once" tag was explained twice**, once for runewords and once for
  uniques. Folded into the single explanation in the Normal section, where a
  reader first meets the tag.
- ***Named items for the small slots*** was merged back into *The six small
  slots*. The armor and helm sections each keep cards and verdict together;
  this should match.

**Gear tab reordered.** The slot sections had been inserted between *Nightmare*
and *Hell*, which split the difficulty arc in half. Order is now: farming order
and Cube mechanics → Normal → Nightmare → **Hell** → armor slot → helm slot →
small slots → Beyond Hell. The difficulty narrative runs uninterrupted, then the
by-slot upgrade reference follows it. All directional cross-references
("above" / "below" / "further down") re-audited after the move.

**Conventions.** 26 literal em-dashes were converted to `&mdash;` per the
AGENTS.md rule; all were pre-existing, in sections untouched this session. The
one inside a CSS comment was left alone. `AGENTS.md` said "five tab panels" and
"click all five tabs" — there have been six since the Prerequisites tab landed.

**Checked and deliberately left alone:** cards for items the guide recommends
*against* (Ormus' Robes, Enigma, Crown of Thieves, Nightwing's Veil). They read
like extras but they are the guide's voice working correctly — it says plainly
when something popular is a bad fit, and cutting them would leave the reader to
rediscover each one.

## Quests that must not be skipped

Once Leaf and Stealth are done it's fine to rush the rest of Normal, except:

- **The Horadric Cube** (Act 2, "The Horadric Staff") — every socket recipe and
  rune upgrade here needs it.
- **Larzuk / "Siege on Harrogath"** (early Act 5, kill Shenk) — this is what
  grants the socket charges the plan counts on, and it's easy to blow past.
- **The Golden Bird** (Act 3) — permanent +20 max life, once per difficulty.
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
