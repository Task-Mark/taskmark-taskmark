---
id: T-103
type: task
title: Hide completed control on all lists
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-094, T-096]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-038
epic: E-010
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
tags: [dashboard, frontend, filters]
created: 2026-07-23
updated: 2026-07-27T07:23:21.914Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 12000
---

# T-103: Hide completed control on all lists

## Description

Add a “Hide completed” toggle that excludes `status: done` rows from Overall epic/story/task lists and Work items.

## Acceptance criteria

- [x] Toggle UI with clear label (e.g. Hide completed).
- [x] When on, rows with status `done` are hidden.
- [x] Applies to epic, story, task, and Work items lists.
- [x] Default off (show completed) unless product decides otherwise — document default **off**.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:03:09Z | prompt | Marco Mendão | implement E-010 list search and filters |
| 2 | 2026-07-23T16:03:09Z | feedback | Marco Mendão | delivered search, parent/tags filters, hide completed |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:01:01Z | shared-batch: 12792 of 140714ms by points; delivered T-103 |
