---
id: T-110
type: task
title: Hide empty General epic and show child progress bars
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-079, T-081]
points: 3
points_source: suggested
estimate_minutes: 48
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: E-008
epic: E-008
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
tags: [dashboard, frontend, general, lists]
created: 2026-07-23
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-23T16:32:13Z
completed_at: 2026-07-23T16:34:23Z
actual_ms: 130000
---
# T-110: Hide empty General epic and show child progress bars

## Description

On Overall lists: hide the General epic when it has no stories and no tasks/bugs. Replace epic and story status cells with a progress bar showing realized (done) children vs total — stories and tasks/bugs for epics; tasks/bugs for stories. Hide-completed continues to filter by the row’s own `status`.

## Acceptance criteria

- [x] General epic is omitted from the epic list when it has zero stories and zero tasks/bugs.
- [x] Epic list Status column shows a progress bar of done stories+tasks/bugs over total (not a bare “done” status badge).
- [x] Story list Status column shows a progress bar of done tasks/bugs over total under that story.
- [x] Hide completed still hides rows whose own status is `done` (unchanged behavior).
- [x] Empty child sets show a clear empty/zero progress state (not a false 100%).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:32:13Z | prompt | Marco Mendão | hide empty General; progress bars instead of complete status; hide toggle unchanged |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 767515a | taskmark-taskmark | 2026-07-23T16:40:51Z | Marco Mendão | complete t-110 progress bars board |
| e3e8c71 | taskmark-frontend | 2026-07-23T16:40:51Z | Marco Mendão | add epic story progress bars |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:32:13Z | 2026-07-23T16:34:23Z | Hide empty General; progress bars on epic/story lists |
