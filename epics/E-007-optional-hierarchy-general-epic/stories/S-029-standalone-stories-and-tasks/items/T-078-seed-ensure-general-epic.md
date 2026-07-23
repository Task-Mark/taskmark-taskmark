---
id: T-078
type: task
title: Seed and ensure General epic on boards
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-028, T-019]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-029
epic: E-007
owner: ""
blocked: false
cancelled: false
tags: [plugin, init, hierarchy]
created: 2026-07-23
updated: 2026-07-23T05:10:21.353Z
started_at: 2026-07-23T04:43:50Z
completed_at: 2026-07-23T04:44:50Z
actual_ms: 60000
---
# T-078: Seed and ensure General epic on boards

## Description

Make `taskmark-init` (and create/sync paths that need it) ensure a default **General** epic exists on every board, including a catch-all story for orphan tasks when required by folder layout.

## Acceptance criteria

- [x] New boards from init include a General epic.
- [x] Create flows that fall back to General create the epic (and catch-all story if needed) when missing.
- [x] Existing boards gain General on first need without duplicating if already present (match by title/slug/tag).
- [x] General is distinguishable in docs/INDEX (e.g. tag or reserved slug).

## Notes



## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T04:38:20Z | prompt | Allow standalone stories/tasks; infer parents from context; default General epic for unattached work |
| 2 | 2026-07-23T04:45:32Z | prompt | Develop S-029 |
| 3 | 2026-07-23T04:45:32Z | feedback | Done as part of S-029 shared batch |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T04:43:50Z | 2026-07-23T04:44:50Z | shared-batch: 1 of 4min by points; delivered T-078 |
