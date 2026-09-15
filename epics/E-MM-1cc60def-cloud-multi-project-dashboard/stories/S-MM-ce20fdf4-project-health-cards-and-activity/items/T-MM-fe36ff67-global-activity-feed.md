---
id: T-MM-fe36ff67
type: task
title: Global activity feed across projects
status: backlog
priority: high
size: S
points: 3
parent: S-MM-ce20fdf4
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, activity]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-fe36ff67: Global activity feed across projects

## Description

Merge the `recentActivity` events of all selected projects, sort by `receivedAt` newest-first, and render them in the visual style of `WorkActivityFeed` with a project badge on each row. Honour the author and project filters.

## Acceptance criteria

- [ ] Recent worklog events from every selected project appear in one feed, newest first.
- [ ] Each row shows actor, item title, summary, time, and a project badge.
- [ ] Author and project filters narrow the feed.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — merged recent activity feed with project badges. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
