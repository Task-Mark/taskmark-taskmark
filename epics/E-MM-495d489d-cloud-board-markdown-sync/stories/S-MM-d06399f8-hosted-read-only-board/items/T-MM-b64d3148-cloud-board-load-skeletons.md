---
id: T-MM-b64d3148
type: task
title: Show skeletons while the cloud board loads
status: done
priority: medium
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
tags: [cloud, ui, loading]
created: 2026-09-03
updated: 2026-09-03T18:22:00Z
started_at: 2026-09-03T18:15:36Z
completed_at: 2026-09-03T18:22:00Z
---
# T-MM-b64d3148: Show skeletons while the cloud board loads

## Description

While Taskmark Cloud is fetching a project board, show layout skeletons that match the board chrome and list instead of a blank page or a text-only loading message.

## Acceptance criteria

- [x] Navigating to a project board shows skeleton placeholders for the app bar actions, heading, metrics, and list until the snapshot is ready.
- [x] Opening project Settings also shows a skeleton while the token page loads.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T18:15:36Z | prompt | Marco Mendão | Add skeletons while the Cloud board is loading. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T18:15:36Z | 2026-09-03T18:22:00Z | Added board and Settings loading skeletons for Cloud project routes. |
