# Signal Status Report — 2026-10-20T22:05Z
> Vague mode. No entry/strategy details. ECN pts basis. $0.10/pt at 0.1 lot.
> OOS period ≈ 3 yrs (2020–23). IS period ≈ 2 yrs (2024–26). Frequency columns are estimates.
> WP/t = net pts/trade (1R=10pt basis). W% columns are stable across time horizons.

## Combined Stack — All Periods

| Branch | Period | n | WR% | PF | WP/w | WP/m | WP/yr | W%/w | W%/m | W%/yr | W%/t | WP/t (pts) | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| #StackC | IS | 152 | 62% | 2.97 | ~1.5 | ~6 | ~76 | 62% | 62% | 62% | 62% | ~7.5 | Best stack |
| #StackC | OOS | 175 | 66% | 2.94 | ~1.1 | ~5 | ~58 | 66% | 66% | 66% | 66% | ~6.6 | Bootstrap P(net<0)=0% |
| #StackA | IS | 164 | 62% | 2.76 | ~1.6 | ~7 | ~82 | 62% | 62% | 62% | 62% | ~6.7 | |
| #StackA | OOS | 182 | 66% | 2.54 | ~1.2 | ~5 | ~61 | 66% | 66% | 66% | 66% | ~5.2 | |

> WP/t formula: (1−WR%) × (PF−1) × 10 pts. At $0.10/pt, 0.1 lot: WP/t($) ≈ WP/t × $0.10.

## Individual Legs — OOS

| Leg | n | WR% | PF | WP/w | WP/m | WP/yr | W%/t | WP/t (pts) | Status |
|---|---|---|---|---|---|---|---|---|---|
| Leg1 (#G11) | 36 | 75% | 5.19 | ~0.2 | ~1 | ~12 | 75% | ~10.5 | ✅ |
| Leg2 (#vgs1b) | 67 | 61% | 1.77 | ~0.4 | ~2 | ~22 | 61% | ~3.0 | ⚠️ marginal PF |
| Leg3 (#T82) | 35 | 60% | 2.21 | ~0.2 | ~1 | ~12 | 60% | ~4.8 | ⚠️ small sample IS |
| Leg4 (#n016) | 44 | 70% | 3.07 | ~0.2 | ~1 | ~15 | 70% | ~6.2 | ✅ |

## Watch List

| Code | n | WR% | PF | WP/w | WP/m | WP/yr | W%/t | WP/t (pts) | Notes |
|---|---|---|---|---|---|---|---|---|---|
| #v2.3 | 32 | ~47% | 6.29 | — | — | — | ~47% | ~28.2 | Venue-only, no OOS yet |
| #v2.4 | 19 | — | 10.33 | — | — | — | — | — | n<30, rejected |

> #v2.3 high WP/t is driven by large PF with sub-50% WR; treat as unconfirmed pending OOS.

*Entry logic and strategy details are private.*
