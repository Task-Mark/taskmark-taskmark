---
id: T-163
type: task
title: Replace app brand logo with tm_light mark
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [T-141]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
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
tags: [app-bar, brand, ui]
created: 2026-07-27
updated: 2026-07-27T05:18:44.416Z
started_at: 2026-07-27T05:13:45Z
completed_at: 2026-07-27T05:16:31Z
actual_ms: 0
---
# T-163: Replace app brand logo with tm_light mark

## Description

Use `public/tm_light.png` as the Taskmark brand logo (with `tm_dark.png` for dark mode). Replace the previous `logo.png` usage in the app bar and apply the mark on the setup screen.

## Acceptance criteria

- [x] App bar shows `tm_light.png` (and dark variant when `.dark`).
- [x] Setup screen shows the same brand mark.
- [x] Old `logo.png` is no longer referenced.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:13:45Z | prompt | Marco Mendão | Use tm_light.png as the logo |
| 2 | 2026-07-27T05:15:09Z | feedback | Marco Mendão | BrandLogo wired; logo.png removed |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| b13c67c | taskmark-frontend | 2026-07-27T06:18:24+01:00 | Marco Mendão | persist hide filters, brand logo, and story progress |
| 3235283 | taskmark-taskmark | 2026-07-27T06:18:25+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Duration | Note |
|---------|-------|---------------|-------------|----------|------|
| 1 | Marco Mendão | 2026-07-27T05:13:45Z | 2026-07-27T05:16:31Z | — | BrandLogo with tm_light/tm_dark; removed logo.png |
