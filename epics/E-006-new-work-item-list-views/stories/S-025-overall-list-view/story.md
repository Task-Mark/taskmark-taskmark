---
id: S-025
type: story
title: Overall list view (current drill-down)
status: done
priority: high
size: S
size_source: rolled_up
size_basis: [sum:tasks]
points: 3
points_source: rolled_up
estimate_minutes: 45
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-006
epic: E-006
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, views, overall]
created: 2026-07-22
updated: 2026-07-23T16:33:36.080Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:42:22Z
actual_ms: 19000
---

# S-025: Overall list view (current drill-down)

## User story

As a user, I want the Overall view to keep today’s epic → story → task drill-down so I can work the board the way I already do.

## Acceptance criteria

- [x] Overall is the default view and shows the existing nested lists.
- [x] Drill-down selection behavior is unchanged in Overall.
- [x] Switching to another view and back to Overall restores the drill-down experience with project context intact.
- [x] Detail sheet still opens from Overall list rows.

## Tasks

- [T-065: Register Overall as default view mode](items/T-065-register-overall-as-default-view.md)
- [T-066: Preserve drill-down under Overall view](items/T-066-preserve-drill-down-under-overall.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-22T00:29:24Z | prompt | Create E-006 new work item list views with stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T06:38:57Z | 2026-07-23T06:38:57Z | shared-batch parent rollup (0ms; effort on child tasks) |
