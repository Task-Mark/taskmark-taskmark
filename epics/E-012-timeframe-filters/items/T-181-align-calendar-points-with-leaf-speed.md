---
id: T-181
type: task
title: Align calendar points with leaf speed logic
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-180, T-173]
points: 2
points_source: suggested
estimate_minutes: 0
actual_minutes: 0
estimate_source: suggested
estimate_basis: []
session_cap_minutes: 480
parent: E-012
epic: E-012
owner: ""
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
tags: [filters, timeframe, calendar, metrics, points]
created: 2026-07-27
updated: 2026-07-27T07:36:40.469Z
started_at: 2026-07-27T07:02:34Z
completed_at: 2026-07-27T07:03:33Z
actual_ms: 59000
---

# T-181: Align calendar points with leaf speed logic

## Description

Make the calendar picker show the same task/bug leaf-point totals used by Current Speed. Stories with sub tasks should not contribute their own story points to the calendar totals.

## Acceptance criteria

- [x] Calendar week/day point totals are based on completed task/bug leaves only.
- [x] Stories are excluded from picker point totals.
- [x] Stories with sub tasks no longer double count points through the story row.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T07:02:34Z | prompt | Marco Mendão | Calendar should match Current Speed using completed task/bug leaf points; stories with sub tasks should not add extra points |
| 2 | 2026-07-27T07:03:33Z | feedback | Marco Mendão | Calendar picker aligned with Current Speed task/bug leaf points |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d5f8f02 | taskmark-frontend | 2026-07-27T07:08:31Z | Marco Mendão | add project metrics and calendar points |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T07:02:34Z | 2026-07-27T07:03:33Z | Calendar picker now matches Current Speed leaf-point totals |
