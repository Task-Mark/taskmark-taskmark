# Team velocity

Last synced: 2026-07-29T07:31:14.976Z
Window: Current Speed 90-day weekly points average (done tasks/bugs by completed_at)

## Throughput

| Metric | Value |
|--------|-------|
| Current Speed (pts/week) | 337 |
| Active weeks in average | 1 |
| Done items in window | 276 |
| Sum points in window | 648 |
| Median points | 3 |
| Median actual_minutes | 12 |
| Median minutes per point | 12 |

## Remaining backlog

| Metric | Value |
|--------|-------|
| Open items (excl. cancelled) | 11 |
| Sum points remaining | 34 |
| Sum estimate_minutes remaining | 405 |
| ETA (calendar weeks @ Current Speed) | ~0.1 weeks |
| ETA (from median min/point) | ~408 min |

## Notes

- **Current Speed** = average weekly story points of done tasks/bugs over 90 days
  anchored at the latest completed leaf. Excludes the **current** ISO week and
  weeks with **0** points (same rule as board UI).
- Suggested Est = points × median min/point when ≥3 trustworthy samples
  (`actual_minutes > 2`) exist in that window (`estimate_basis: [speed:90d:Nmin/pt]`).
- Calendar ETA = remaining points ÷ Current Speed (weeks).
