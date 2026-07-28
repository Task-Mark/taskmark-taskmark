---
id: B-008
type: bug
title: Brand logo sits flush against app bar bottom border
status: done
priority: medium
size: XL
size_source: suggested
size_basis: [calibrated:B-008]
points: 8
points_source: suggested
estimate_minutes: 480
actual_minutes: 480
estimate_source: suggested
estimate_basis: [calibrated:B-008]
session_cap_minutes: 480
parent: S-003
epic: E-001
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
tags: [frontend, app-bar, ui]
created: 2026-07-27
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-27T08:59:14Z
completed_at: 2026-07-28T06:19:44Z
actual_ms: 28800000
---
# B-008: Brand logo sits flush against app bar bottom border

## Description

The `tm_light` / `tm_dark` brand mark in the sticky app bar sits visually against the header bottom border. The artwork has almost no bottom padding in the PNG, so with the current header vertical padding the mark looks glued to the line under the header.

## Repro steps

1. Open the board UI with the app bar visible.
2. Look at the Taskmark brand mark on the left of the header.
3. Observe the bottom of the mark sits flush against the header bottom border.

## Fix criteria

- [x] Clear visual breathing room between the brand mark and the header bottom border (including on hover scale).
- [x] Header layout otherwise unchanged (project switcher, add project).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T08:59:14Z | prompt | Marco Mendão | Imagem da equipa no cabeçalho colada à linha em baixo — resolver espaçamento |
| 2 | 2026-07-28T06:19:44Z | feedback | Marco Mendão | Close B-008 — logo spacing fix accepted |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| cb6c435 | taskmark-frontend | 2026-07-28T06:18:39Z | Marco Mendão | remove overall est actual columns |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T08:59:14Z | 2026-07-28T06:19:44Z | Increased app-bar bottom padding and logo margin so mark clears header border |
