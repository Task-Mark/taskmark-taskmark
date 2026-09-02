---
id: T-MM-fb640cb4
type: task
title: Add ProjectSyncToken and SyncTokenGuard
status: done
priority: high
size: M
points: 5
parent: S-MM-54ca5d61
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
tags: [api, auth, sync]
created: 2026-09-02
updated: 2026-09-02T18:07:57Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-fb640cb4: Add ProjectSyncToken and SyncTokenGuard

## Description

Store one opaque `tmk_` sync token per project, expose get and rotate over cookie auth, and resolve bearer tokens to a project id for CLI sync routes.

## Acceptance criteria

- [x] `GET /v1/projects/:projectId/sync-token` returns the current token for an active member, creating it if missing.
- [x] `POST /v1/projects/:projectId/sync-token/rotate` is owner-only and invalidates the previous token.
- [x] A SyncTokenGuard maps `Authorization: Bearer` to project id without requiring a project id in the request.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: one recoverable project token that local instances use as TASKMARK_SYNC_TOKEN. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Added ProjectSyncToken, get/rotate endpoints, and SyncTokenGuard. |
