---
id: E-007
type: epic
title: Optional hierarchy and General epic
status: backlog
priority: high
size: null
size_source: rolled_up
size_basis: [sum:stories]
points: 13
points_source: rolled_up
estimate_minutes: 195
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:stories]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
blocked: false
cancelled: false
tags: [plugin, conventions, hierarchy, dashboard]
created: 2026-07-23
updated: 2026-07-23T04:38:56.857Z
started_at: null
completed_at: null
actual_ms: 0
---
# E-007: Optional hierarchy and General epic

## Goal

Let stories and tasks exist without a required parent, while still preferring a contextual epic/story when one is clear, and house truly unattached work under a default **General** epic visible in the epic list.

## Scope

- Optional `parent` / `epic` for stories and tasks (null allowed).
- Create skills infer parents from prompt/context when the user does not name one.
- Fallback attachment to a board-default **General** epic (and a catch-all story under it when a task has no story).
- Dashboard epic list always includes General so unattached work is discoverable.
- Conventions, init, create skills, and UI/parser updates needed for the above.

## Out of scope

- Deleting or flattening existing epic → story → task trees.
- Free-form items outside the board markdown model.
- Renaming or merging user epics into General automatically.

## Success metrics

- Creating a story or task without an explicit parent succeeds.
- Unattached items appear under General in the epic list.
- Explicit or clearly contextual parents still win over General.

## Stories

- [S-029: Standalone stories and tasks with General epic](stories/S-029-standalone-stories-and-tasks/story.md)

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
