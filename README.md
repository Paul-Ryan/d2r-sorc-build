# How to build a Sorceress in Diablo 2: Resurrected

Fire Ball → Frozen Orb hybrid Sorceress build reference for Diablo II: Resurrected.

**Live:** https://www.paul-ryan.online/d2r-sorc-build/

Single-file static site (`index.html`, no build step, no dependencies). Deployed
automatically to GitHub Pages on every push to `main`.

## Layout

Content is split across six tabs, each linkable by hash:

| Tab | Hash | Covers |
| --- | --- | --- |
| Skill Points | `#points` | Quest points, the leveling rail, the real build's fill order, Static Field |
| Gear | `#gear` | Farming order, the Cube & crafting, sockets, runewords by difficulty, then gear by slot |
| Stats & Keys | `#stats` | Stat budget and allocation, controller layout |
| Mercenary | `#merc` | Aura choice, Insight → Infinity, why he dies, merc helm & armor |
| Breakpoints & Resists | `#numbers` | FCR/FHR tables, the Hell resist penalty |
| Prerequisites | `#prereq` | Expansion vs Classic, online vs offline, accounts, connection, how to play, trading on Xbox |

Light and dark themes follow the OS by default; the header toggle overrides and
persists to `localStorage`. Printing flattens every tab onto one page.

## Docs

Working notes for editing this guide, kept out of the page itself:

- [AGENTS.md](AGENTS.md) — how `index.html` is structured, its component
  vocabulary, and the conventions to match.
- [docs/build-facts.md](docs/build-facts.md) — the settled numbers and decisions
  behind the guide, with the reasoning that produced them.
- [docs/sources.md](docs/sources.md) — which D2 reference sites are actually
  reachable, their URL patterns, and where they disagree.

## Skill allocation, resolved

**Fire Bolt, not Fire Mastery.** Fire damage is `base x (1 + synergies) x (1 + mastery)`,
and the two brackets multiply rather than adding. Synergies count **hard points only** --
gear, charms and shrines never raise them -- while Fire Mastery is a skill whose own level
*does* scale with `+skills`.

That asymmetry front-loads Fire Mastery brutally: its first point is worth +30% (more once
your +5 to +7 skills are counted), and every point after it is worth roughly +4%. A Fire
Bolt point is a flat +14% and is unaffected by gear, so it out-earns a second Fire Mastery
point until Fire Bolt is around 18.

The plan therefore takes **Fire Bolt to 20 and Fire Mastery to 6-11**, rather than the
reverse. For the same points that is roughly 35% more Fire Ball damage, and it closes the
old 6-11 point surplus to exactly zero -- the surplus was an artifact of over-funding
Fire Mastery.

**Still open:** Cold Mastery 10 vs 15, which trades directly against Fire Mastery 11 vs 6.
Worth about +17% fire damage either way -- not decisive, and best settled at the Monarch
respec with real gear in hand.

## Local preview

```
python3 -m http.server 4173
```

Then open http://localhost:4173.
