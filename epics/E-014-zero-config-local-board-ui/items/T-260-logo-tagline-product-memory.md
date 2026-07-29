---
id: T-260
type: task
title: Replace logo subtitle with product memory tagline
status: done
priority: medium
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 25
actual_minutes: 1
estimate_source: suggested
estimate_basis: [speed:90d:13min/pt]
session_cap_minutes: 480
parent: E-014
epic: E-014
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
tags: [frontend, branding, ui]
created: 2026-07-29
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-29T07:08:36Z
completed_at: 2026-07-29T07:13:00Z
actual_ms: 60000
---
# T-260: Replace logo subtitle with product memory tagline

## Description

In the application logo / app-bar brand area, replace the dynamic subtitle that shows counts like `X projects · X workspaces` with the fixed tagline **Product memory for agent work**.

## Acceptance criteria

- [x] Logo / brand chrome no longer shows project or workspace counts.
- [x] Subtitle text is exactly `Product memory for agent work`.
- [x] Change appears in local board UI (`@taskmark/ui` / `npx taskmark serve`) and any shared app-bar that uses the same logo block.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T05:50:53Z | prompt | Marco Mendão | In the logo instead of X projects · X workspaces write "Product memory for agent work" |
| 2 | 2026-07-29T07:08:36Z | prompt | Marco Mendão | implement T-260, T-261 and T-262 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T07:08:36Z | 2026-07-29T07:09:36Z | shared-batch: 1 of 4min by points — Product memory tagline on brand chrome |
