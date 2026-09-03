---
id: T-MM-a43006c1
type: task
title: Select or create a project from the cloud board picker
status: done
priority: high
size: M
points: 5
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
tags: [cloud, ui, projects]
created: 2026-09-03
updated: 2026-09-03T18:20:00Z
started_at: 2026-09-03T14:28:14Z
completed_at: 2026-09-03T14:31:58Z
---
# T-MM-a43006c1: Select or create a project from the cloud board picker

## Description

Replace the conditional native project select with an always-visible Taskmark project picker that lists every active project associated with the signed-in account and includes a create-project action in the same flow.

## Acceptance criteria

- [x] The cloud board always shows the selected project in a project picker, including accounts with one project.
- [x] The picker lists all active projects returned for the signed-in user and navigates to the selected board.
- [x] The same picker opens a create-project form, reports validation or API errors, and switches to the newly created project on success.
- [x] An account with no projects can create its first project instead of seeing a dead-end empty state.
- [x] Cloud lint and production build pass.
- [x] The project picker sits directly beside Log out in the cloud app bar.
- [x] Short project lists do not show a scrollbar; long lists remain scrollable.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T18:20:00Z | prompt | Marco Mendão | Remove the owner role label from the Taskmark Cloud app bar. |
| 2026-09-03T14:55:25Z | feedback | Marco Mendão | Place the dropdown beside Log out and remove the scrollbar that appears when hovering a short project list. |
| 2026-09-03T14:28:14Z | prompt | Marco Mendão | Add a cloud board project picker that lets users select any associated board and create a new project. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T18:20:00Z | 2026-09-03T18:20:00Z | Removed the membership role label from the Cloud app bar. |
| Marco Mendão | 2026-09-03T14:28:14Z | 2026-09-03T14:31:58Z | Replaced the conditional select with an always-visible project picker and integrated first-project creation and switching. |
| Marco Mendão | 2026-09-03T14:55:25Z | 2026-09-03T14:55:25Z | Moved the picker beside Log out and limited scrolling to project lists longer than six entries. |
