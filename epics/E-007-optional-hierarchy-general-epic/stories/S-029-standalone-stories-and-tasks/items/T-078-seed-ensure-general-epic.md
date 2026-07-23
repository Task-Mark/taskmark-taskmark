---
id: T-078
type: task
title: Seed and ensure General epic on boards
status: backlog
priority: high
size: S
size_source: suggested
size_basis: [T-028, T-019]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
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
updated: 2026-07-23T04:38:56.857Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-078: Seed and ensure General epic on boards

## Description

Make `taskmark-init` (and create/sync paths that need it) ensure a default **General** epic exists on every board, including a catch-all story for orphan tasks when required by folder layout.

## Acceptance criteria

- [ ] New boards from init include a General epic.
- [ ] Create flows that fall back to General create the epic (and catch-all story if needed) when missing.
- [ ] Existing boards gain General on first need without duplicating if already present (match by title/slug/tag).
- [ ] General is distinguishable in docs/INDEX (e.g. tag or reserved slug).

## Notes



## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T04:38:20Z | prompt | Allow standalone stories/tasks; infer parents from context; default General epic for unattached work |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
