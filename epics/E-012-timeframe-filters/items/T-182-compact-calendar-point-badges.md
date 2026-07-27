---
id: T-182
type: task
title: Compact calendar point badges
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [T-180]
points: 1
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
tags: [filters, timeframe, calendar, formatting]
created: 2026-07-27
updated: 2026-07-27T07:06:27.645Z
started_at: 2026-07-27T07:06:11Z
completed_at: 2026-07-27T07:06:27Z
actual_ms: 16000
---

# T-182: Compact calendar point badges

## Description

Format large calendar point totals compactly so values like 1000 render as 1K in picker badges.

## Acceptance criteria

- [x] Day point badges use compact formatting for large values.
- [x] Week point badges use the same compact formatting.
- [x] Tooltip/title still exposes the full point total.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T07:06:11Z | prompt | Marco Mendão | In the calendar, large numbers like 1000 should render as 1K |
| 2 | 2026-07-27T07:06:27Z | feedback | Marco Mendão | Calendar badge totals now compact-format large values like 1K |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d5f8f02 | taskmark-frontend | 2026-07-27T07:08:31Z | Marco Mendão | add project metrics and calendar points |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T07:06:11Z | 2026-07-27T07:06:27Z | Compact point badges added for day and week calendar totals |
