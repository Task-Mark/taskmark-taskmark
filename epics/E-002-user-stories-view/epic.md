---
id: E-002
type: epic
title: User stories view
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 11
points_source: rolled_up
estimate_minutes: 1265
actual_minutes: 831
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [dashboard, stories, frontend]
created: 2026-07-21
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-21T17:45:49Z
completed_at: 2026-07-21T18:02:46Z
actual_ms: 49878000
estimate_source: rolled_up
---
# E-002: User stories view

## Goal

Let users drill from an epic into its user stories, then from a selected story into the tasks connected to that story—so the dashboard shows the full epic → story → task hierarchy.

## Scope

- Select an epic (from the existing epic list or an epic picker) and show all user stories under that epic.
- Select a user story and show all tasks (and bugs) connected to that story.
- Parse story and item markdown from the local Taskmark board for the active project.
- Present id, title, status, size, points, and related summary fields for stories and tasks.
- Empty and error states when an epic has no stories or a story has no items.

## Out of scope

- Editing board files from the UI.
- Creating or reordering stories/tasks in the UI.
- Full markdown body / work-log detail panes (beyond list summary fields).
- Cross-project story views (stories are scoped to the selected epic’s project board).

## Success metrics

- From the dashboard, a user can pick an epic and see every story under it.
- Selecting a story reveals its connected tasks/bugs without leaving the drill-down flow.
- Parse failures for individual files do not break the whole view.

## Stories

- [S-005: Story list for selected epic](stories/S-005-story-list-for-epic/story.md)
- [S-006: Task list for selected story](stories/S-006-task-list-for-story/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| a940d8b | taskmark-frontend | 2026-07-21T17:43:42Z | Marco Mendão | add e-002 user stories view board |
| 10d1691 | taskmark-cursor | 2026-07-21T17:43:42Z | Marco Mendão | add e-002 user stories view board |
| 0c104cd | taskmark-frontend | 2026-07-21T17:59:56Z | Marco Mendão | add story list for selected epic |
| 2aef6ba | taskmark-cursor | 2026-07-21T17:59:56Z | Marco Mendão | sync taskmark board |
| 4e49022 | taskmark-frontend | 2026-07-21T22:21:39Z | Marco Mendão | add task list for selected story |
| ca69fce | taskmark-cursor | 2026-07-21T22:21:39Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T04:11:46Z | 2026-07-21T10:02:46Z | auto-backfilled: rollup from children (missing/under-logged) |
| 2 | Marco Mendão | 2026-07-21T10:02:46Z | 2026-07-21T18:02:46Z | auto-backfilled: rollup from children (missing/under-logged) |
