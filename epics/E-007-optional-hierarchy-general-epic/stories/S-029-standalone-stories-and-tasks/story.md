---
id: S-029
type: story
title: Standalone stories and tasks with General epic
status: backlog
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 13
points_source: rolled_up
estimate_minutes: 195
actual_minutes: 0
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-007
epic: E-007
owner: ""
blocked: false
cancelled: false
tags: [plugin, conventions, hierarchy, create]
created: 2026-07-23
updated: 2026-07-23T04:38:56.857Z
started_at: null
completed_at: null
actual_ms: 0
---
# S-029: Standalone stories and tasks with General epic

## User story

As a user, I want to create stories without an epic and tasks without a story when I do not have a clear parent, and still see that work under a default General epic, so I can capture work quickly without inventing hierarchy first.

## Acceptance criteria

- [ ] A story can exist with `parent`/`epic` null (or attached only to General).
- [ ] A task/bug can exist without a user-created story/epic (housed under General when needed).
- [ ] When the user does not name a parent, create skills try to assign an epic/story from prompt and board context.
- [ ] When no clear parent fits, unattached stories/tasks live under the default **General** epic.
- [ ] The epic list always shows General so unattached work is visible.

## Tasks

- [T-076: Conventions for optional parents and General epic](items/T-076-conventions-optional-parents-general.md)
- [T-077: Soft-attach create-story and create-task](items/T-077-soft-attach-create-skills.md)
- [T-078: Seed and ensure General epic on boards](items/T-078-seed-ensure-general-epic.md)
- [T-079: Show General epic with unattached items in UI](items/T-079-ui-general-epic-unattached.md)

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
