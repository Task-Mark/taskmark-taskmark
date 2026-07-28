---
id: S-029
type: story
title: Standalone stories and tasks with General epic
status: done
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 15
points_source: rolled_up
estimate_minutes: 230
actual_minutes: 40
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-007
epic: E-007
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
tags: [plugin, conventions, hierarchy, create]
created: 2026-07-23
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-23T04:41:50Z
completed_at: 2026-07-23T04:45:50Z
actual_ms: 2426000
---

# S-029: Standalone stories and tasks with General epic

## User story

As a user, I want to create stories without an epic and tasks without a story when I do not have a clear parent, and still see that work under a default General epic, so I can capture work quickly without inventing hierarchy first.

## Acceptance criteria

- [x] A story can exist with `parent`/`epic` null (or attached only to General).
- [x] A task/bug can exist without a user-created story/epic (housed under General when needed).
- [x] When the user does not name a parent, create skills try to assign an epic/story from prompt and board context.
- [x] When no clear parent fits, unattached stories/tasks live under the default **General** epic.
- [x] The epic list always shows General so unattached work is visible.

## Tasks

- [B-005: Tasks and bugs cannot live under an epic without a story](items/B-005-epic-direct-tasks-without-story.md)

- [T-076: Conventions for optional parents and General epic](items/T-076-conventions-optional-parents-general.md)
- [T-077: Soft-attach create-story and create-task](items/T-077-soft-attach-create-skills.md)
- [T-078: Seed and ensure General epic on boards](items/T-078-seed-ensure-general-epic.md)
- [T-079: Show General epic with unattached items in UI](items/T-079-ui-general-epic-unattached.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T04:38:20Z | prompt | Marco Mendão | Allow standalone stories/tasks; infer parents from context; default General epic for unattached work |
| 2 | 2026-07-23T04:41:50Z | prompt | Marco Mendão | Develop S-029 (standalone stories/tasks + General epic) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| dbb8838 | taskmark-cursor | 2026-07-23T05:20:13Z | Marco Mendão | epic-direct tasks drop unattached story |
| cd914a9 | taskmark-frontend | 2026-07-23T05:20:13Z | Marco Mendão | show general tasks under epics |
| 6aae4fd | taskmark-taskmark | 2026-07-23T05:20:14Z | Marco Mendão | remove unattached story fix b-005 |
| 571e51a | taskmark-cursor | 2026-07-23T04:47:21Z | Marco Mendão | add optional parents and general epic |
| b1d87ab | taskmark-frontend | 2026-07-23T04:47:21Z | Marco Mendão | show general epic first in list |
| f3c7b3e | taskmark-taskmark | 2026-07-23T04:47:21Z | Marco Mendão | complete s-029 optional hierarchy board |
| 23411cb | taskmark-taskmark | 2026-07-23T04:41:03Z | Marco Mendão | add e-007 optional hierarchy board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T04:41:50Z | 2026-07-23T04:41:50Z | shared-batch parent rollup (0 min); leaves hold effort |
| 2 | Marco Mendão | 2026-07-23T04:41:03Z | 2026-07-23T05:20:14Z | auto-recovered: commit span |
