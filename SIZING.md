# T-shirt sizing and story points

| Size | Points | Meaning | Seed estimate |
|------|--------|---------|---------------|
| XS | 1 | Trivial | 16 min |
| S | 2 | Small | 32 min |
| M | 3 | Medium | 48 min |
| L | 5 | Large | 2 days |
| XL | 8 | Extra large (prefer split) | 3+ days |

Weights for size rollups: XS=1, S=2, M=3, L=4, XL=5.

Seed estimates are calibrated from **AI-assisted billable work-log minutes** (and commit-span recovery when logs undercount). Effort uses **billable work-log minutes** only (idle auto-cap: next-day 12:00 UTC; session cap default 480). Never use calendar span.

## Calibration log

| Date | Item | Sized | Points | Est | Actual | Note |
|------|------|-------|--------|-----|--------|------|
| 2026-07-21 | T-048 | M | 3 | 50 | 3 | estimate 50->5; size M->XS |
| 2026-07-21 | T-049 | S | 2 | 30 | 3 | estimate 30->5; size S->XS |
| 2026-07-21 | T-050 | S | 2 | 30 | 3 | estimate 30->5; size S->XS |
| 2026-07-21 | T-051 | M | 3 | 50 | 3 | estimate 50->5; size M->XS |
| 2026-07-21 | T-052 | S | 2 | 30 | 3 | estimate 30->5; size S->XS |
| 2026-07-21 | T-053 | S | 2 | 30 | 3 | estimate 30->5; size S->XS |
| 2026-07-21 | T-054 | M | 3 | 50 | 3 | estimate 50->5; size M->XS |
| 2026-07-21 | T-055 | M | 3 | 50 | 3 | estimate 50->5; size M->XS |
| 2026-07-21 | T-056 | S | 2 | 30 | 3 | estimate 30->5; size S->XS |
| 2026-07-21 | T-057 | M | 3 | 50 | 3 | estimate 50->5; size M->XS |
| 2026-07-21 | T-058 | S | 2 | 30 | 3 | estimate 30->5; size S->XS |
| 2026-07-21 | T-059 | M | 3 | 50 | 3 | estimate 50->5; size M->XS |
| 2026-07-21 | T-060 | S | 2 | 30 | 3 | estimate 30->5; size S->XS |
| 2026-07-21 | B-003 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-001 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-003 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-004 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-008 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | B-001 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-005 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-007 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-017 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-018 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | B-002 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-020 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-021 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-023 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-024 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-025 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-026 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-027 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-028 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-029 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-031 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-032 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-033 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-034 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-035 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-036 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-037 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-038 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-039 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-040 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-041 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-042 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-043 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-044 | M | 3 | 480 | 48 | estimate 480->50 |
| 2026-07-21 | T-045 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-046 | S | 2 | 120 | 32 | estimate 120->30 |
| 2026-07-21 | T-016 | S | 2 | 120 | 261 | estimate 120->260 |
| 2026-07-21 | T-011 | M | 3 | 480 | 16 | estimate 480->15; size M->XS |
| 2026-07-21 | T-012 | M | 3 | 480 | 16 | estimate 480->15; size M->XS |
| 2026-07-21 | T-013 | S | 2 | 120 | 16 | estimate 120->15; size S->XS |
| 2026-07-21 | T-006 | M | 3 | 480 | 46 | estimate 480->45; size M->XS |
| 2026-07-21 | T-002 | S | 2 | 120 | 14 | estimate 120->15; size S->XS |
| 2026-07-21 | T-009 | M | 3 | 480 | 14 | estimate 480->15; size M->XS |
| 2026-07-21 | T-010 | S | 2 | 120 | 14 | estimate 120->15; size S->XS |
