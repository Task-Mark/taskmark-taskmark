---
id: T-MM-581394b8
type: task
title: Show and rotate the project sync token in Settings
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
tags: [cloud, ui, settings]
created: 2026-09-02
updated: 2026-09-02T18:07:57Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-581394b8: Show and rotate the project sync token in Settings

## Description

Add a project Settings tab in taskmark-cloud where members copy the sync token and owners rotate it, with setup copy for `TASKMARK_SYNC_TOKEN`.

## Acceptance criteria

- [x] Settings shows the current token with a copy control and env-var setup instructions.
- [x] Owners can rotate the token after a warning that existing local instances will fail until they update the env var.
- [x] Non-owners can copy the token but cannot rotate it.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: Settings tab so members copy the project token and send it to other developers. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Added the cloud Settings tab to copy and rotate the sync token. |
