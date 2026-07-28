---
id: T-140
type: task
title: Week range dual dropdown instead of slider
status: done
priority: medium
size: S
size_source: suggested
size_basis: [velocity:similar]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
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
tags: [filters, timeframe, weeks, frontend, ui]
created: 2026-07-24
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-24T16:57:13Z
completed_at: 2026-07-24T16:58:20Z
actual_ms: 67000
---

# T-140: Week range dual dropdown instead of slider

## Description

Replace the week-range slider with a dual dropdown combo that reads like an input mask (`W12 – W18`).

## Acceptance criteria

- [x] Week range mode uses from/to week selects, not a slider.
- [x] Controls appear as a single combo / input-mask style group.
- [x] From/to stay ordered (from ≤ to).

## Notes

Follow-up polish on E-012.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T16:57:13Z | prompt | Marco Mendão | Week range should be dual dropdown combo like input mask, not slider |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d010f70 | taskmark-frontend | 2026-07-24T17:00:20Z | Marco Mendão | use dual week dropdown for range filter |
| efa533f | taskmark-taskmark | 2026-07-24T17:00:20Z | Marco Mendão | complete t-140 week range dual dropdown |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:57:13Z | 2026-07-24T16:58:20Z | replaced week range slider with Wfrom–Wto select combo |
