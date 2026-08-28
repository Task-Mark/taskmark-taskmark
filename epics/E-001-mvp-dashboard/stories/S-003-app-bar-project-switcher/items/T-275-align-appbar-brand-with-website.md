---
id: T-275
type: task
title: Align website header brand with frontend app bar
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-163, T-260]
points: 2
points_source: suggested
estimate_minutes: 25
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:12min/pt]
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
tags: [app-bar, brand, ui, frontend]
created: 2026-07-29
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-29T10:30:58Z
completed_at: 2026-07-29T11:30:07Z
actual_ms: 47000
---
# T-275: Align website header brand with frontend app bar

## Description

Make the marketing website site header brand lockup match the local board UI app bar (logo, wordmark hover underline, and Product memory tagline). Frontend is the source of truth.

## Acceptance criteria

- [x] Website SiteHeader brand lockup matches frontend AppBar (logo + Taskmark wordmark with hover underline/rotate).
- [x] Website header shows the tagline Product memory for agent work.
- [x] Frontend app bar branding is restored (not simplified to the old website header).
- [x] Brand remains readable on light and dark surfaces.


## Notes

Source of truth: taskmark-frontend AppBar. Target: taskmark-website SiteHeader.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T10:30:58Z | prompt | Marco Mendão | App bar logo branding on taskmark-frontend should match taskmark-website |
| 2 | 2026-07-29T10:31:45Z | feedback | Marco Mendão | App bar now mirrors website header brand lockup |
| 3 | 2026-07-29T11:30:07Z | prompt | Marco Mendão | Other way around: frontend logo branding should be used on website; restore frontend from commits |
| 4 | 2026-07-29T11:30:07Z | feedback | Marco Mendão | Restored frontend AppBar; applied same lockup to website SiteHeader |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T10:30:58Z | 2026-07-29T10:31:45Z | Matched app bar brand lockup to website SiteHeader (logo + Taskmark wordmark) |
| 2 | Marco Mendão | 2026-07-29T11:30:07Z | 2026-07-29T11:30:07Z | Restored frontend brand; applied AppBar lockup to website header |
