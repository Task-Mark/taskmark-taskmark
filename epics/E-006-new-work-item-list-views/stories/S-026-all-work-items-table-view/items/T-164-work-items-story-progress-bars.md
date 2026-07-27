---
id: T-164
type: task
title: Show story progress bars on Work items list
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [T-110]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-026
epic: E-006
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
tags: [dashboard, frontend, views, progress]
created: 2026-07-27
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-27T05:16:08Z
completed_at: 2026-07-27T05:18:44Z
actual_ms: 0
---
# T-164: Show story progress bars on Work items list

## Description

On the Work items tab, user stories should show the same child progress bar used on Overall (done/total of tasks and bugs under the story), instead of only a status badge.

## Acceptance criteria

- [x] Story rows with child work items show `ChildProgressBar` (done/total).
- [x] Epic-direct tasks/bugs and stories with zero children still show status (+ solved tooltip).
- [x] Matches Overall work items progress behavior for stories.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:16:08Z | prompt | Marco Mendão | Work items list should show progress bars on user stories |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| b13c67c | taskmark-frontend | 2026-07-27T06:18:24+01:00 | Marco Mendão | persist hide filters, brand logo, and story progress |
| 3235283 | taskmark-taskmark | 2026-07-27T06:18:25+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Duration | Note |
|---------|-------|---------------|-------------|----------|------|
| 1 | Marco Mendão | 2026-07-27T05:16:08Z | 2026-07-27T05:18:44Z | — | Story progress bars on Work items list |
