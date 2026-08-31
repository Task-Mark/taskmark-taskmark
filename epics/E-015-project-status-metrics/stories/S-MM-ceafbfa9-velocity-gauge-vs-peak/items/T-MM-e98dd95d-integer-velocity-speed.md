---
id: T-MM-e98dd95d
type: task
title: Show velocity speed as a whole number
status: done
priority: medium
size: XS
points: 1
parent: S-MM-ceafbfa9
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
tags: [frontend, metrics, velocity]
created: 2026-08-31
updated: 2026-08-31T11:12:20Z
started_at: 2026-08-31T11:10:33Z
completed_at: 2026-08-31T11:12:20Z
---

# T-MM-e98dd95d: Show velocity speed as a whole number

Round Current Speed and peak speed on the Velocity card to the nearest integer before display. A value such as 228.2 must appear as 228 on the gauge label, the peak subtitle, and the exact title/accessible name. Compact magnitudes (1K, 1M) still apply after rounding. Complete work items and Current week stay unchanged.

## Acceptance criteria

- [x] The Velocity gauge center value is a whole number (228.2 displays as 228).
- [x] The peak subtitle uses the same integer rounding.
- [x] Title and accessible name for the velocity speed are integers as well.
- [x] Compact abbreviations still apply to rounded values of 1000 or more.
- [x] Complete work items and Current week formatting is unchanged.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T11:10:33Z | prompt | Marco Mendão | Velocity metrics should show an integer speed; 228.2 must round to 228. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T11:10:33Z | 2026-08-31T11:12:20Z | Rounded Velocity current and peak speed labels to whole numbers |
