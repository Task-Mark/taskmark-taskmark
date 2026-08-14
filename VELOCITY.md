# Team velocity

Last synced: 2026-08-14T17:50:46.835Z
Window: Current Speed 90-day weekly points average (done tasks/bugs by completed_at)

## Throughput

| Metric | Value |
|--------|-------|
| Current Speed (pts/week) | 325 |
| Active weeks in average | 2 |
| Done items in window | 279 |
| Sum points in window | 655 |
| Median points | 3 |
| Median actual_minutes | 12 |
| Median minutes per point | 12 |

## Remaining backlog

| Metric | Value |
|--------|-------|
| Open items (excl. cancelled) | 14 |
| Sum points remaining | 42 |
| Sum estimate_minutes remaining | 500 |
| ETA (calendar weeks @ Current Speed) | ~0.1 weeks |
| ETA (from median min/point) | ~504 min |

## Notes

- **Current Speed** = average weekly story points of done tasks/bugs over 90 days
  anchored at the latest completed leaf. Excludes the **current** ISO week and
  weeks with **0** points (same rule as board UI).
- Suggested Est = points × median min/point when ≥3 trustworthy samples
  (`actual_minutes > 2`) exist in that window (`estimate_basis: [speed:90d:Nmin/pt]`).
- Calendar ETA = remaining points ÷ Current Speed (weeks).
