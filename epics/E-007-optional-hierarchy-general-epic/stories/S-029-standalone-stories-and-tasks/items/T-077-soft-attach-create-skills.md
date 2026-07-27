---
id: T-077
type: task
title: Soft-attach create-story and create-task
status: done
priority: high
size: L
size_source: suggested
size_basis: [T-028, T-044]
points: 5
points_source: suggested
estimate_minutes: 75
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-029
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
tags: [plugin, skills, create, hierarchy]
created: 2026-07-23
updated: 2026-07-27T07:09:18.868Z
started_at: 2026-07-23T04:42:50Z
completed_at: 2026-07-23T04:43:50Z
actual_ms: 60000
---
# T-077: Soft-attach create-story and create-task

## Description

Change `create-story` and `create-task` so a parent is preferred but not required: if the user does not name an epic/story, infer from prompt and open board context; otherwise attach under **General** (creating a catch-all story under General when a task has no story).

## Acceptance criteria

- [x] `create-story` succeeds without an explicit epic; prefers contextual epic, else General.
- [x] `create-task` succeeds without an explicit story; prefers contextual story/epic, else General + catch-all story.
- [x] Explicit parent ids/titles from the user always win.
- [x] Skills and project-memory rules no longer block creation when no parent is named.
- [x] Reply still reports assigned parent/epic (including General when used).

## Notes

Keep sync-status / rollups working when General holds mixed unattached work.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T04:38:20Z | prompt | Marco Mendão | Allow standalone stories/tasks; infer parents from context; default General epic for unattached work |
| 2 | 2026-07-23T04:45:32Z | prompt | Marco Mendão | Develop S-029 |
| 3 | 2026-07-23T04:45:32Z | feedback | Marco Mendão | Done as part of S-029 shared batch |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T04:42:50Z | 2026-07-23T04:43:50Z | shared-batch: 1 of 4min by points; delivered T-077 |
