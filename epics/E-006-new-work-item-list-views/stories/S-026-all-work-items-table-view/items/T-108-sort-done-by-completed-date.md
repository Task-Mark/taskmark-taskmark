---
id: T-108
type: task
title: Sort done work items by completed date
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-067]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-026
epic: E-006
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
tags: [dashboard, frontend, lists, sorting]
created: 2026-07-23
updated: 2026-07-23T17:36:48Z
started_at: 2026-07-23T16:18:57Z
completed_at: 2026-07-23T16:21:07Z
actual_ms: 130000
---

# T-108: Sort done work items by completed date

## Description

Within Work items (and any list using `compareByStatusThenPriority`), sort done/solved rows by `completed_at` (newest first) instead of `created`. Open rows keep created-date ordering.

## Acceptance criteria

- [x] Done rows sort by completed date descending (missing completed_at falls back reasonably).
- [x] Non-done rows still sort by created date descending within their status/priority group.
- [x] Work items list description reflects the sort rule.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:18:57Z | prompt | Marco Mendão | solved issues sorted by done date not create date |
| 2 | 2026-07-23T16:21:07Z | feedback | Marco Mendão | compareByStatusThenPriority uses completedAt for done |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9f8fe9a | taskmark-frontend | 2026-07-23T16:28:18Z | Marco Mendão | sort done work items by solved date |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:18:57Z | 2026-07-23T16:21:07Z | Sort done rows by completedAt |
