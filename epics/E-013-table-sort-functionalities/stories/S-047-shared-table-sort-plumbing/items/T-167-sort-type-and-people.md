---
id: T-167
type: task
title: Sort by type and people
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-166]
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
updated: 2026-07-27T05:34:38Z
started_at: 2026-07-27T05:29:14Z
completed_at: 2026-07-27T05:30:00Z
actual_ms: 0
---
# T-167: Sort by type and people

## Description

Extend table sort with **type** (epic/story/task/bug) and **people** (contributor names), wired on lists that show those columns.

## Acceptance criteria

- [x] `type` sorts epic < story < task < bug.
- [x] `people` sorts by unique contributor names (empty last).
- [x] Type header on overall, task, and work items lists.
- [x] People header on all board lists that show the People column.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:29:14Z | prompt | Marco Mendão | People and type sortable as well |
| 2 | 2026-07-27T05:30:00Z | feedback | Marco Mendão | Type and people sort keys wired |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Duration | Note |
|---------|-------|---------------|-------------|----------|------|
| 1 | Marco Mendão | 2026-07-27T05:29:14Z | 2026-07-27T05:30:00Z | — | Type + people sort |
