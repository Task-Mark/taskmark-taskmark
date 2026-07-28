---
id: T-138
type: task
title: Scroll week picker to current week; distinct prev/next colors
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [velocity:similar]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
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
started_at: 2026-07-24T16:25:50Z
completed_at: 2026-07-24T16:26:21Z
actual_ms: 31000
---

# T-138: Scroll week picker to current week; distinct prev/next colors

## Description

On open, scroll/focus the week list on the current ISO week. Give previous and next weeks different background treatments from each other and from Now.

## Acceptance criteria

- [x] Opening the week dropdown scrolls the current week into view and focuses it.
- [x] Previous, current, and next weeks use distinct background styles.

## Notes

Follow-up polish on E-012.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T16:25:50Z | prompt | Marco Mendão | Open focused on current week; different backgrounds for prev vs next |
| 2 | 2026-07-24T16:27:30Z | prompt | Marco Mendão | Prev/next same background with more opacity |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:25:50Z | 2026-07-24T16:26:21Z | scroll/focus current week; distinct prev/now/next backgrounds |
