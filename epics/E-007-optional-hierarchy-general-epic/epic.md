---
id: E-007
type: epic
title: Optional hierarchy and General epic
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 16
points_source: rolled_up
estimate_minutes: 200
actual_minutes: 7
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
blocked: false
cancelled: false
tags: [plugin, conventions, hierarchy, dashboard]
created: 2026-07-23
updated: 2026-07-23T05:21:40Z
started_at: 2026-07-23T04:41:50Z
completed_at: 2026-07-23T04:45:50Z
actual_ms: 420000
---
# E-007: Optional hierarchy and General epic

## Goal

Let stories and tasks exist without a required parent, while still preferring a contextual epic/story when one is clear, and house general tasks and user stories under a default **General** epic visible in the epic list.

## Scope

- Optional `parent` / `epic` for stories and tasks (null allowed).
- Create skills infer parents from prompt/context when the user does not name one.
- Fallback attachment to a board-default **General** epic (and a catch-all story under it when a task has no story).
- Dashboard epic list always includes General so general tasks and user stories are discoverable.
- Conventions, init, create skills, and UI/parser updates needed for the above.

## Out of scope

- Deleting or flattening existing epic → story → task trees.
- Free-form items outside the board markdown model.
- Renaming or merging user epics into General automatically.

## Success metrics

- Creating a story or task without an explicit parent succeeds.
- General tasks and user stories appear under General in the epic list (epic `items/` + stories; no Unattached story).
- Explicit or clearly contextual parents still win over General.

## Stories

- [S-029: Standalone stories and tasks with General epic](stories/S-029-standalone-stories-and-tasks/story.md)

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| dbb8838 | taskmark-cursor | 2026-07-23T05:20:13Z | epic-direct tasks drop unattached story |
| cd914a9 | taskmark-frontend | 2026-07-23T05:20:13Z | show general tasks under epics |
| 6aae4fd | taskmark-taskmark | 2026-07-23T05:20:14Z | remove unattached story fix b-005 |
| 571e51a | taskmark-cursor | 2026-07-23T04:47:21Z | add optional parents and general epic |
| b1d87ab | taskmark-frontend | 2026-07-23T04:47:21Z | show general epic first in list |
| f3c7b3e | taskmark-taskmark | 2026-07-23T04:47:21Z | complete s-029 optional hierarchy board |
| 23411cb | taskmark-taskmark | 2026-07-23T04:41:03Z | add e-007 optional hierarchy board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T04:41:50Z | 2026-07-23T04:41:50Z | shared-batch parent rollup (0 min) |
