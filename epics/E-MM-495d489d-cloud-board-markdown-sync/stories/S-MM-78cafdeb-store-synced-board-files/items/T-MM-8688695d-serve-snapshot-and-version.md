---
id: T-MM-8688695d
type: task
title: Serve board snapshot and version to the cloud app
status: done
priority: high
size: S
points: 3
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
tags: [api, cloud]
created: 2026-09-02
updated: 2026-09-02T18:07:57Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-8688695d: Serve board snapshot and version to the cloud app

## Description

Expose cookie-authenticated snapshot and version reads for project members so the cloud UI can render and poll for updates.

## Acceptance criteria

- [x] `GET /v1/boards/:projectId/snapshot` returns the stored snapshot for an active member.
- [x] `GET /v1/boards/:projectId/version` returns the current version for cheap polling.
- [x] Missing boards return a clear empty state payload rather than leaking other projects.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: cookie-auth snapshot and version endpoints for the hosted board. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Added cookie-auth snapshot and version reads for members. |
