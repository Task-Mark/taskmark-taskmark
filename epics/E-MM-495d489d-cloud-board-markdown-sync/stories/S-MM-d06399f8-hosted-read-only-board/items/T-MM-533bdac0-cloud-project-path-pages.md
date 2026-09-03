---
id: T-MM-533bdac0
type: task
title: Address each cloud project at a path page
status: done
priority: high
size: S
points: 3
parent: S-MM-d06399f8
epic: E-MM-495d489d
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
tags: [cloud, ui, routing]
created: 2026-09-03
updated: 2026-09-03T18:22:00Z
started_at: 2026-09-03T18:15:36Z
completed_at: 2026-09-03T18:22:00Z
---
# T-MM-533bdac0: Address each cloud project at a path page

## Description

Replace query-string project selection (`?project=…`) with a real path for each Cloud project, such as `/6a998b4d316ab817e74f7c6d`, and keep Settings on that same project path.

## Acceptance criteria

- [x] Opening a Cloud project uses `/{projectId}` instead of `/?project=`.
- [x] Project picker, create-project, Settings, and Board links stay on the path-based URLs.
- [x] `/` with no projects still shows the create-first-project state; `/` with projects redirects to a project path.
- [x] Legacy `/?project=` and `/settings?project=` URLs redirect to the path pages.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T18:15:36Z | prompt | Marco Mendão | Use a real /{projectId} page on Taskmark Cloud instead of ?project= query selection. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T18:15:36Z | 2026-09-03T18:22:00Z | Replaced query-string project selection with /{projectId} board pages and /{projectId}/settings. |
