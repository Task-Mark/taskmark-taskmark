---
id: T-MM-e519b03b
type: task
title: Replace detail sheet tables with mobile log cards
status: done
priority: high
size: M
points: 5
parent: S-018
epic: E-005
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
tags: [dashboard, frontend, sheet, detail, mobile, responsive]
created: 2026-09-01
updated: 2026-09-01T06:47:35Z
started_at: 2026-09-01T06:44:10Z
completed_at: 2026-09-01T06:47:35Z
---

# T-MM-e519b03b: Replace detail sheet tables with mobile log cards

## Description

Make every tabular section in the work-item detail sheet readable on narrow screens without horizontal scrolling. Below the `sm` breakpoint, render Prompt & feedback, Commits, Work log, and any GFM tables embedded in prose as compact semantic cards. Prioritize each log row's summary or message and present supporting fields as labelled metadata. Keep the existing dense tables on larger screens and preserve empty states, dates, work-item links, and all parsed values.

## Acceptance criteria

- [x] Prompt & feedback, Commits, Work log, and GFM prose tables contain no visible table on mobile and require no horizontal scrolling
- [x] Each mobile card gives the summary or commit message visual priority and presents every applicable table field with a clear label
- [x] Aggregated parent rows retain their linked work-item badges and all detail types use the same responsive behavior
- [x] Desktop and tablet layouts from `sm` upward retain the existing tables
- [x] Empty states remain clear and the frontend typecheck, tests, and production build pass

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-01T06:44:10Z | prompt | Marco Mendão | /tkmd-plan-do: replace every table in the work-item detail sheet on mobile with a responsive div-based alternative using the best practical UI and UX. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-01T06:44:10Z | 2026-09-01T06:47:35Z | Replaced detail log tables and embedded prose tables with labelled mobile cards while retaining desktop tables; lint, 50 tests, and production build passed. |
