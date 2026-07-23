---
id: T-077
type: task
title: Soft-attach create-story and create-task
status: backlog
priority: high
size: L
size_source: suggested
size_basis: [T-028, T-044]
points: 5
points_source: suggested
estimate_minutes: 75
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-029
epic: E-007
owner: ""
blocked: false
cancelled: false
tags: [plugin, skills, create, hierarchy]
created: 2026-07-23
updated: 2026-07-23T04:38:56.857Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-077: Soft-attach create-story and create-task

## Description

Change `create-story` and `create-task` so a parent is preferred but not required: if the user does not name an epic/story, infer from prompt and open board context; otherwise attach under **General** (creating a catch-all story under General when a task has no story).

## Acceptance criteria

- [ ] `create-story` succeeds without an explicit epic; prefers contextual epic, else General.
- [ ] `create-task` succeeds without an explicit story; prefers contextual story/epic, else General + catch-all story.
- [ ] Explicit parent ids/titles from the user always win.
- [ ] Skills and project-memory rules no longer block creation when no parent is named.
- [ ] Reply still reports assigned parent/epic (including General when used).

## Notes

Keep sync-status / rollups working when General holds mixed unattached work.

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
