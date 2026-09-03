---
id: T-MM-8bc96943
type: task
title: Persist and expose project worklog activity
status: done
priority: high
size: M
points: 5
parent: S-MM-bc1935b3
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
tags: [api, mongodb, worklog, activity]
created: 2026-09-03
updated: 2026-09-03T18:54:00Z
started_at: 2026-09-03T18:41:51Z
completed_at: 2026-09-03T18:54:00Z
---
# T-MM-8bc96943: Persist and expose project worklog activity

## Description

Accept work-log activity on board sync, retain a bounded recent project feed, and expose it to authenticated project members.

## Acceptance criteria

- [x] Board sync validates optional work-log activity events.
- [x] Board state stores a bounded, deduplicated recent activity list.
- [x] Project members can read activity through `GET /v1/boards/:projectId/activity`.
- [x] Non-members cannot read project activity.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T18:41:51Z | prompt | Marco Mendão | Save and implement compact API storage and polling for recent work-log activity. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T18:41:51Z | 2026-09-03T18:54:00Z | Stored bounded recent activity on board sync and exposed GET activity for members. |
