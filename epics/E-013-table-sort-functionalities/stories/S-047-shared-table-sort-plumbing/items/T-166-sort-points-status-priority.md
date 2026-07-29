---
id: T-166
type: task
title: Sort by points, status, and priority
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-142, T-165]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-047
epic: E-013
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
tags: [dashboard, frontend, lists, sort]
created: 2026-07-27
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-27T05:27:49Z
completed_at: 2026-07-27T05:28:30Z
actual_ms: 0
---
# T-166: Sort by points, status, and priority

## Description

Extend shared table sort so lists can sort by **points**, **status**, and **priority** (where those columns appear), using the same three-click cycle as other columns.

## Acceptance criteria

- [x] Sort keys include `points`, `status`, and `priority`.
- [x] Points sort numerically (nulls last).
- [x] Status uses workflow rank (backlog → in_progress → done → …).
- [x] Priority uses urgency rank (critical → high → medium → low).
- [x] Headers wired on lists that show those columns (epics: points; overall/story/task: points+status; work items: points+status+priority).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:27:49Z | prompt | Marco Mendão | Also sortable by points, status, and priority |
| 2 | 2026-07-27T05:28:30Z | feedback | Marco Mendão | Extended sort keys and wired list headers |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Duration | Note |
|---------|-------|---------------|-------------|----------|------|
| 1 | Marco Mendão | 2026-07-27T05:27:49Z | 2026-07-27T05:28:30Z | — | Points/status/priority sort keys and headers |
