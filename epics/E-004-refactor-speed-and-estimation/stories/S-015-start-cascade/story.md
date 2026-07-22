---
id: S-015
type: story
title: Start cascade for task, story, epic
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 80
actual_minutes: 80
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [start-work, cascade, status]
created: 2026-07-21
updated: 2026-07-22T00:16:21.562Z
started_at: 2026-07-21T21:47:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 4800000
---
# S-015: Start cascade for task, story, epic

## User story

As a user or agent, I want a start action on tasks, stories, and epics so started_at is set, and starting a task also starts its parent story and epic if they have not started.

## Acceptance criteria

- [x] Start action exists for task, story, and epic (skill/command).
- [x] Starting a task sets task.started_at and, if null, story.started_at and epic.started_at.
- [x] Starting a story sets story.started_at and epic.started_at if null.
- [x] Opens work-log session where appropriate (task/bug); does not invent closed micro-sessions.

## Tasks

- [T-040: Start task cascades to story and epic](items/T-040-start-task-cascade-parents.md)
- [T-041: Start actions for story and epic](items/T-041-start-story-epic-actions.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:56:48Z | prompt | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |
| 2 | 2026-07-21T23:07:27Z | feedback | E-004 dual model delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T21:47:27Z | 2026-07-21T23:07:27Z | auto-backfilled: velocity × points (missing work log) |

