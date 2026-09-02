---
id: T-MM-6d867bbf
type: task
title: Persist files and snapshot through board-sync endpoints
status: done
priority: high
size: L
points: 8
parent: S-MM-78cafdeb
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
tags: [api, sync]
created: 2026-09-02
updated: 2026-09-02T18:07:57Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-6d867bbf: Persist files and snapshot through board-sync endpoints

## Description

Add BoardFile and BoardState models and token-authenticated manifest and sync endpoints that accept relative markdown files plus a snapshot cache.

## Acceptance criteria

- [x] `GET /v1/board-sync/manifest` returns path hashes plus project name and slug.
- [x] `PUT /v1/board-sync` upserts or deletes allowed paths, stores the snapshot, and increments version.
- [x] Path, size, and batch limits reject unsafe payloads; e2e tests cover the happy path and unauthorized access.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: files as source of truth plus snapshot cache, with the token selecting the project. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Added board-sync manifest/PUT endpoints with file and snapshot storage. |
