# Paul's Diablo II: Resurrected Sorceress Build Guide

Fire Ball → Frozen Orb hybrid Sorceress build reference for Diablo II: Resurrected.

**Live:** https://www.paul-ryan.online/d2r-sorc-build/

Single-file static site (`index.html`, no build step, no dependencies). Deployed
automatically to GitHub Pages on every push to `main`.

## Layout

Content is split across five tabs, each linkable by hash:

| Tab | Hash | Covers |
| --- | --- | --- |
| Skill Point Ledger | `#points` | Quest math, Phases 1–3, Static Field, the Ice Bolt verdict |
| Stats & Keys | `#stats` | Stat budget and allocation, controller layout |
| Gear | `#gear` | Runewords, getting sockets, gear by slot, shopping order by difficulty |
| Breakpoints & Resists | `#numbers` | FCR/FHR tables, the Hell resist penalty |
| Mercenary | `#merc` | Aura choice, Insight → Infinity, merc gear |

Light and dark themes follow the OS by default; the header toggle overrides and
persists to `localStorage`. Printing flattens every tab onto one page.

## Open decision

**Fire Bolt.** It is Fire Ball's synergy at +14% fire damage per level and currently
sits at the 1-point prerequisite. The 6–11 point surplus cannot max it, but can take
it to level 7–12 for roughly +84% to +154% — the best remaining use of those points,
since Static Field wants exactly one and Warmth and Energy Shield want none. The
tradeoff is holding Cold Mastery at 10 instead of 15. Deliberately unresolved: the
Monarch respec reopens the whole skill tree, so it can be settled then.

## Local preview

```
python3 -m http.server 4173
```

Then open http://localhost:4173.
