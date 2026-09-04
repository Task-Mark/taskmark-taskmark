---
id: T-MM-8a532434
type: task
title: Persist presence on board state and tick every 30 minutes
status: done
priority: high
size: M
points: 5
parent: S-MM-f998c021
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
tags: [api, presence, activity]
created: 2026-09-03
updated: 2026-09-04T08:31:39Z
started_at: 2026-09-03T21:56:00Z
completed_at: 2026-09-03T22:02:00Z
---
# T-MM-8a532434: Persist presence on board state and tick every 30 minutes

## Description

Store presence cards on `BoardState` separately from `recentActivity`. On member `GET /v1/boards/:projectId/activity`, claim a 30-minute tick with a conditional `findOneAndUpdate` so only one concurrent poll runs the refresh. Each tick refreshes actors with worklogs since the previous tick, plus anyone with stored worklogs but no card yet. Cards never expire: a person's card stays until a newer summary replaces it. Return `{ recent, presence }`.

## Acceptance criteria

- [x] `BoardState` stores `presenceTickedAt` and `presence` cards with id, actor, summary, generatedAt, and sourceEventIds.
- [x] `GET /v1/boards/:projectId/activity` returns `presence` alongside `recent` and does not write presence into `recentActivity`.
- [x] A tick runs at most once per 30 minutes per board, even when Cloud polls every few seconds.
- [x] Only actors with new worklogs since the last tick get a replaced card; anyone with worklogs but no card yet also gets one, and existing cards never expire.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T08:31:39Z | prompt | Marco Mendão | A summary message must always be visible and may only disappear when a newer one replaces it. |
| 2026-09-03T21:56:00Z | prompt | Marco Mendão | Cursor plan: persist presence on board state and lazily tick every 30 minutes on activity GET. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-04T08:31:00Z | 2026-09-04T08:31:39Z | Dropped the two-hour expiry so each person's summary stays until a newer one replaces it. |
| Marco Mendão | 2026-09-03T21:56:00Z | 2026-09-03T22:02:00Z | Stored presence on BoardState and claimed a 30-minute tick on activity GET. |
