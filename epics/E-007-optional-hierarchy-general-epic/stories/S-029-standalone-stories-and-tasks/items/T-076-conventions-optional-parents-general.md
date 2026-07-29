---
id: T-076
type: task
title: Conventions for optional parents and General epic
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-026, T-044]
points: 3
points_source: suggested
estimate_minutes: 45
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
tags: [plugin, conventions, hierarchy]
created: 2026-07-23
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-23T04:41:50Z
completed_at: 2026-07-23T04:42:50Z
actual_ms: 60000
---
# T-076: Conventions for optional parents and General epic

## Description

Update Taskmark conventions (frontmatter, folder layout, templates, INDEX notes) so stories may omit an epic and tasks may omit a story, and document the reserved default **General** epic as the home for unattached stories/tasks.

## Acceptance criteria

- [x] Frontmatter docs allow `parent`/`epic` null for stories and for tasks/bugs when using General fallback paths.
- [x] Folder layout documents where General and its catch-all story/items live.
- [x] Templates and quick rules no longer require a hard parent for every story/task.
- [x] General epic naming/slug and “do not delete / always present” rules are documented.

## Notes

Physical files still live under an epic/story path when attached to General; “standalone” means optional *user* hierarchy, not free-floating files outside `epics/`.

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
| 1 | Marco Mendão | 2026-07-23T04:41:50Z | 2026-07-23T04:42:50Z | shared-batch: 1 of 4min by points; delivered T-076 |
