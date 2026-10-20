# Signal Project — Performance Summary

_Last updated: 2026-10-20. Validated: cycles 33-39, net of costs. Units: ECN pts ($0.10/pt at 0.1 lot). Past results are not advice._

## Pre-Rd40 Reference Entry Revalidation (2026-10-20)

_Re-run with correct first-bar-of-week/day anchors, cost 11pt, directional 1-bar. IS=2024–2026, OOS=2020–2023. All short-side entries._
_Status: PASS = full PF ≥ 1.10 AND OOS PF ≥ 1.10; WEAK = full passes but OOS < 1.10; FAIL = full PF < 1.10._

| Code | Full WR | Full N | Full PF | IS WR | IS N | IS PF | OOS WR | OOS N | OOS PF | Status |
|------|---------|--------|---------|-------|------|-------|--------|-------|--------|--------|
| WedH13H4Bear | 50.1% | 840 | 1.04 | 44.4% | 171 | 0.59 | 51.8% | 199 | 1.14 | WEAK |
| WedH13H4Bear2PriorBull | 52.6% | 135 | 0.93 | 40.9% | 22 | 0.25 | 58.8% | 34 | 1.89 | FAIL |
| T30_WeekUp_H4B_H13_PB | 51.5% | 452 | 1.11 | 47.8% | 90 | 0.67 | 53.7% | 108 | 1.08 | WEAK |
| T33_WeekUp_H4B_H13_2PB | 52.6% | 135 | 0.93 | 40.9% | 22 | 0.25 | 58.8% | 34 | 1.89 | FAIL |
| T34_WeekUp_H4B_H14 | 46.2% | 833 | 0.77 | 50.0% | 168 | 0.88 | 44.9% | 198 | 0.73 | FAIL |
| T35_DualCtx_H4B_H13 | 51.2% | 295 | 0.98 | 48.5% | 66 | 0.87 | 55.7% | 70 | 0.91 | FAIL |
| T36_DualCtx_H4B_H13_PB | 50.0% | 206 | 0.89 | 51.0% | 51 | 0.75 | 53.3% | 45 | 0.81 | FAIL |
| T42_WeekUp_H4B_H13_MWT | 47.8% | 515 | 0.83 | 44.0% | 100 | 0.54 | 47.9% | 119 | 0.91 | FAIL |
| T44_DualCtx_H4B_H13_MWT | 46.5% | 187 | 0.73 | 43.9% | 41 | 0.91 | 47.8% | 46 | 0.50 | FAIL |
| T45_DualCtx_H4B_H13_PB_MWT | 43.3% | 127 | 0.61 | 44.8% | 29 | 0.65 | 43.8% | 32 | 0.41 | FAIL |
| T46_WeekUp_H4B_H13_PB_MWT | 48.9% | 276 | 0.82 | 46.9% | 49 | 0.51 | 48.5% | 68 | 0.76 | FAIL |
| T47_DualCtx_H4B_H13_WT | 48.4% | 122 | 0.70 | 40.0% | 25 | 0.81 | 52.9% | 34 | 0.65 | FAIL |
| T49_WeekUp_H4B_H13_Wed | 50.0% | 182 | 0.84 | 42.9% | 35 | 0.37 | 60.0% | 45 | 2.22 | FAIL |
| T52_DualCtx_H4B_H13_Mon | 43.1% | 65 | 0.81 | 50.0% | 16 | 1.16 | 33.3% | 12 | 0.23 | FAIL |
| T54_DualCtx_H4B_H13_PB_Wed | 42.2% | 45 | 0.52 | 37.5% | 8 | 0.41 | 53.8% | 13 | 0.73 | FAIL |
| T56_WeekUp_H4B_H13_PB_Thu | 51.2% | 80 | 1.02 | 50.0% | 14 | 0.92 | 36.0% | 25 | 0.42 | FAIL |
| T57_DualCtx_H4B_H13_PB_WT | 42.9% | 84 | 0.52 | 38.9% | 18 | 0.55 | 48.0% | 25 | 0.47 | FAIL |
| T81_WeekUp_H4B_H13_PB_WT | 50.0% | 186 | 0.81 | 45.7% | 35 | 0.43 | 50.9% | 53 | 0.82 | FAIL |
| T84D_WeekUp_H4B_H13_H11B_Thu | 56.2% | 48 | 1.50 | 42.9% | 7 | 3.27 | 44.4% | 9 | 0.87 | WEAK |
| T90_H23_WeekDown_Wed | 29.1% | 196 | 0.60 | 35.1% | 37 | 1.83 | 18.8% | 48 | 0.22 | FAIL |
| allow_h05h09 | 41.1% | 8482 | 0.67 | 41.0% | 1469 | 0.62 | 42.9% | 2059 | 0.67 | FAIL |
| skip_h16h19 | 41.9% | 35975 | 0.73 | 41.2% | 6762 | 0.65 | 41.7% | 8807 | 0.70 | FAIL |
| MonGapUpFade | 47.7% | 300 | 0.86 | 41.9% | 62 | 0.29 | 53.6% | 84 | 1.22 | FAIL |

_T85, T86, T88, T97, T101 not in archive — filter definitions needed to run._
_T90 IS anomaly (PF=1.83) is IS-only artefact; OOS collapses to 0.22 — discard._
_T49 OOS PF=2.22 is OOS-only; IS fails badly (0.37) — not reliable._
_T84-D full PF=1.50 but very small N (48 total, 9 OOS) — no statistical weight._

**Verdict:** Zero pre-Rd40 entries survive both IS and OOS thresholds at 11pt cost with correct anchors. All are REFERENCE ONLY — do not use for live decisions.

## Post-Rd40 Validated Entries — OOS Coverage Status

_Entries run with correct anchors and pkl post-Round 40. OOS = 2020–2023 unless noted._

| Code | OOS present | Notes |
|------|-------------|-------|
| T133 | TBD | Confirm from gate_candidates.md |
| T142 | TBD | Confirm from gate_candidates.md |
| T144s / SetA | TBD | Confirm from gate_candidates.md |
| T153 | TBD | Confirm from gate_candidates.md |
| T155 | TBD | Confirm from gate_candidates.md |
| T164 | TBD | Confirm from gate_candidates.md |
| T169 | TBD | Confirm from gate_candidates.md |
| T171 / SetB | Yes | battery_ASK_UTC_h11*.md has OOS split |
| T196 | TBD | Confirm from gate_candidates.md |
| T202 / SetD | TBD | Confirm from gate_candidates.md |
| T224 / SetE | TBD | Confirm from gate_candidates.md |
| T250 | TBD | Confirm from gate_candidates.md |

## Combined Stack + Individual Legs (Unified)

_WP = net pts. /t = per trade, /w = per week, /m = per month, /yr = per year. % gain = cumulative on $1,000 base (0.1 lot)._

| Row | Period | n | WR | PF | Net | WP/t | WP/w | WP/m | WP/yr | % gain | Max DD |
|-----|--------|---|----|----|-----|------|------|------|-------|--------|--------|
| **Stack** | IS 2024-26 | 164 | 62% | 2.76 | $1,090 | ~66 | ~87 | ~361 | ~4,330 | 109% | $100 |
| **Stack** | OOS 2020-23 | 182 | 66% | 2.54 | $1,989 | ~109 | ~99 | ~413 | ~4,960 | 199% | $122 |
| **Stack** | All 2020-26 | 346 | 64% | 2.61 | $3,079 | ~89 | ~88 | ~367 | ~4,400 | 308% | $122 |
| Leg 1 | IS | 34 | 71% | 2.84 | — | ~81 | ~22 | ~92 | ~1,102 | — | — |
| Leg 1 | OOS | 36 | 75% | 5.19 | — | ~177 | ~32 | ~133 | ~1,593 | — | — |
| Leg 2 | IS | 57 | 56% | 2.53 | — | ~44 | ~20 | ~84 | ~1,003 | — | — |
| Leg 2 | OOS | 67 | 61% | 1.77 | — | ~67 | ~22 | ~94 | ~1,122 | — | — |
| Leg 3 | IS | 28 | 57% | 3.56 | — | ~55 | ~12 | ~51 | ~616 | — | — |
| Leg 3 | OOS | 35 | 60% | 2.21 | — | ~100 | ~18 | ~73 | ~875 | — | — |
| Leg 4 | IS | 45 | 67% | 2.67 | — | ~90 | ~32 | ~135 | ~1,620 | — | — |
| Leg 4 | OOS | 44 | 70% | 3.07 | — | ~126 | ~28 | ~116 | ~1,386 | — | — |

All 7 years positive.

## Latest Build (pending full confirmation)

| Period | n | WR | PF | Net | WP/t | WP/w | WP/m | WP/yr | % gain | Max DD |
|--------|---|----|----|-----|------|------|------|-------|--------|--------|
| IS 2024-26 | 152 | ~62% | 2.97 | $859 | ~56 | ~68 | ~283 | ~3,436 | 86% | $76 |
| OOS 2020-23 | 175 | ~66% | 2.94 | $1,785 | ~102 | ~89 | ~371 | ~4,463 | 179% | $92 |

_WP estimates use avg pts derived from net $ at 0.1 lot. Individual Leg net not tracked separately. Entry logic and strategy details are private._
