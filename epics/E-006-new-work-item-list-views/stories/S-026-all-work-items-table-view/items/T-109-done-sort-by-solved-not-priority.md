---
id: T-109
type: task
title: Done work items sort by solved date only
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-108]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
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
tags: [dashboard, frontend, lists, sorting]
created: 2026-07-23
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-23T16:24:32Z
completed_at: 2026-07-23T16:26:42Z
actual_ms: 130000
---
# T-109: Done work items sort by solved date only

## Description

Done/cancelled Work items must ignore priority and order solely by solved date (`completed_at`), newest first.

## Acceptance criteria

- [x] Within done (and cancelled), sort by completedAt descending only — priority does not affect order.
- [x] Open statuses still use priority then created.
- [x] Newest solved appears first among solved rows.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:24:32Z | prompt | Marco Mendão | done workitems ordered by solved date not priority |
| 2 | 2026-07-23T16:26:42Z | feedback | Marco Mendão | skip priority for done cohort |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 83957ad | taskmark-taskmark | 2026-07-23T16:28:18Z | Marco Mendão | complete t-108 t-109 done sort rules |
| 9f8fe9a | taskmark-frontend | 2026-07-23T16:28:18Z | Marco Mendão | sort done work items by solved date |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:24:32Z | 2026-07-23T16:26:42Z | Done rows sort by solved date only |
