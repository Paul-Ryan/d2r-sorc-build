# Where to look game facts up

Every source below was fetched and checked on **2026-09-09**. The point of this
file is to skip the trial and error: several obvious-looking D2 sites can't be
read at all, and the ones that can don't always agree.

## Game version this guide targets

D2R is on the **Reign of the Warlock** expansion (released 2026-02-11), engine
version **3.3**, ladder **Season 15**. Nothing in that expansion changed the
Sorceress skills, runewords, or breakpoints this guide is built on — it added
the Warlock class, new Terror Zones and bosses, a loot filter, and some unique
rings. Treat that as true until a patch note says otherwise, and re-check if a
number here ever looks off.

Patch notes: <https://www.icy-veins.com/d2/news/> or Blizzard's official notes.

## Sources that work

### diablo2.io — primary

**This is the site to use.** It is the "diablo.io" that comes up in
conversation, and it *is* fetchable, contrary to earlier assumptions. Data is
kept current to v3.3.

URL patterns — predictable enough to construct directly without searching:

```
https://diablo2.io/runewords/                       index, filterable
https://diablo2.io/runewords/spirit-t3.html         <name-hyphenated>-t<id>.html
https://diablo2.io/runewords/ancients-pledge-t46.html
https://diablo2.io/runewords/rhyme-t1194.html
https://diablo2.io/runewords/splendor-t1222.html
https://diablo2.io/runewords/enigma-t42.html
https://diablo2.io/skills/                          index
https://diablo2.io/skills/static-field-t4165.html   same pattern
https://diablo2.io/skills/teleport-t4176.html
https://diablo2.io/base/kite-shield-t1436.html      base items
https://diablo2.io/base/monarch-t1438.html
https://diablo2.io/base/bone-shield-t1439.html
https://diablo2.io/uniques/lidless-wall-t846.html   uniques
```

There are also `/base/` and `/uniques/` trees on the same pattern. **Base pages
are the best source for socket questions** — each one has an explicit
`Max sockets` field, plus required strength, quality level, the
exceptional/elite upgrades in its family, and which runewords the base accepts.
That last list is the fastest way to answer "what can I put this in".

Base items within a family are numbered consecutively (Kite Shield t1436 →
Dragon Shield t1437 → Monarch t1438), so once you have one id you can usually
walk to its upgrades.

The `t<id>` is a forum topic id and is **not** derivable from the name — the
ids are unordered (Spirit is t3, Blizzard is t9, Static Field is t4165). If you
don't know the id, fetch the index page or web-search
`site:diablo2.io <thing>`.

Runeword pages give runes in order, required level, base item types, the full
stat list split by base (sword vs. shield for Spirit), and patch/ladder status.
Skill pages give class, required level, tree, prerequisites, and synergies.

### d2runewizard.com — breakpoints and cross-checks

<https://d2runewizard.com/breakpoints> renders full per-class FCR and FHR
tables as real HTML. **This is where the Breakpoints & Resists tab's numbers
come from, and it matches them exactly.** Also has a runeword list at
`/runewords` that fetches cleanly.

### diablo2.wiki.fextralife.com — backup

Fetches fine. Good for a second opinion on item stats; thinner on mechanics.
Pattern is `https://diablo2.wiki.fextralife.com/<Name>` (title-case, `+` for
spaces: `/Faster+Cast+Rate`).

### WebSearch

Works and is the fastest way to find a `t<id>` or confirm a patch fact. Search
results alone are not a citation — open the page.

## Sources that don't work

Don't waste fetches on these:

| Source | What happens |
| --- | --- |
| `diablo.io` | Parked domain. No game content. The site people mean is **diablo2.io**. |
| `diablo2.diablowiki.net` | HTTP 403. |
| `maxroll.gg/d2/getting-started/...`, `/d2/resources/breakpoints` | 404 — Maxroll moves URLs often. `/d2/resources/breakpoints-animations` did fetch, but see the disagreement below. |
| `theamazonbasin.com` | Expired TLS certificate. |

## Where sources disagree

**Breakpoint frame counts.** Maxroll and d2runewizard publish different
numbers for the same thresholds. The *thresholds* agree — 0 / 9 / 20 / 37 / 63
/ 105 / 200 FCR — but Maxroll's frame counts run ten lower (13 frames at 0%
where d2runewizard says 23), and its FHR table is offset by a row. Different
counting conventions, not different game behavior.

**This guide follows d2runewizard**: FCR 23 frames at 0% down to 17 at 200%,
FHR 15 frames at 0% down to 7 at 86%. If you're comparing against something
that says 13 frames, it's the other convention — don't "fix" the tables.

The guide also omits the last two FHR rows (142% → 6 frames, 280% → 5). That's
deliberate; they're unreachable for this build.

**Spirit's magic absorb.** diablo2.io lists `+3-8 Magic Absorb`; the guide's
card says `Magic Damage Absorb 3-8%`. Same roll range, different wording, and
worth pinning down properly the next time that card is touched.

**Shield socket maximums.** General web search returns garbage here — results
claimed Kite Shield has 3 sockets *and* that Large Shield maxes at 2, from the
same query, and confused normal/exceptional/elite tiers throughout. **Use the
diablo2.io `/base/` pages instead**; they state `Max sockets` per tier
explicitly. Verified: Kite Shield 3, Bone Shield 2, Grim Shield 2, Monarch 4.

## How to use these when editing

1. Check [build-facts.md](build-facts.md) first — the fact may already be
   settled there, with the reasoning.
2. Fetch diablo2.io for anything about a specific item or skill.
3. Fetch d2runewizard for breakpoints.
4. If the two disagree, say so in the guide rather than silently picking one.
5. When you land a fact that took real work to find, add it to build-facts.md
   so the next session doesn't repeat the search.
