---
id: T-076
type: task
title: Conventions for optional parents and General epic
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-026, T-044]
points: 3
points_source: suggested
estimate_minutes: 45
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-029
epic: E-007
owner: ""
blocked: false
cancelled: false
tags: [plugin, conventions, hierarchy]
created: 2026-07-23
updated: 2026-07-23T04:38:56.857Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-076: Conventions for optional parents and General epic

## Description

Update Taskmark conventions (frontmatter, folder layout, templates, INDEX notes) so stories may omit an epic and tasks may omit a story, and document the reserved default **General** epic as the home for unattached stories/tasks.

## Acceptance criteria

- [ ] Frontmatter docs allow `parent`/`epic` null for stories and for tasks/bugs when using General fallback paths.
- [ ] Folder layout documents where General and its catch-all story/items live.
- [ ] Templates and quick rules no longer require a hard parent for every story/task.
- [ ] General epic naming/slug and “do not delete / always present” rules are documented.

## Notes

Physical files still live under an epic/story path when attached to General; “standalone” means optional *user* hierarchy, not free-floating files outside `epics/`.

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
