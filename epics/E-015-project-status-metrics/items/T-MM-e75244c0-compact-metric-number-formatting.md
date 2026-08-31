---
id: T-MM-e75244c0
type: task
title: Compact large numbers on metric cards
status: done
priority: medium
size: S
points: 3
parent: E-015
epic: E-015
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [frontend, metrics, formatting]
created: 2026-08-31
updated: 2026-08-31T11:07:01Z
started_at: 2026-08-31T11:01:00Z
completed_at: 2026-08-31T11:07:01Z
---

# T-MM-e75244c0: Compact large numbers on metric cards

Show large values on the Overall metrics strip with short magnitude abbreviations (1K, 1M, 1B) so Complete work items, Current week, and Velocity stay readable when counts or points grow large. Reuse the same compact style already used on calendar point badges. Leave contributors and the heatmap unchanged.

## Acceptance criteria

- [x] Complete work items formats each side of `total/complete` with compact magnitudes (for example `1.2K/800` or `1M/999K`).
- [x] Current week formats its point total the same way.
- [x] Velocity formats the current speed label and the peak subtitle the same way.
- [x] Values below 1000 stay as ordinary numbers; thousands use K, millions M, billions B, with at most one decimal.
- [x] Exact values remain available (for example via `title` / accessible name) so compact labels are not the only representation.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T11:01:00Z | prompt | Marco Mendão | Metrics on Complete work items, Current week, and Velocity should format large numbers as 1K, 1M, and similar magnitude abbreviations. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T11:01:00Z | 2026-08-31T11:07:01Z | Compact metric numbers (1K/1M/1B) on Complete, Current week, and Velocity |
