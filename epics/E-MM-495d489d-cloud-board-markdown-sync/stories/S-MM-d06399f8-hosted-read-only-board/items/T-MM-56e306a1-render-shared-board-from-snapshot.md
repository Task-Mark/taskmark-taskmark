---
id: T-MM-56e306a1
type: task
title: Render the shared board from the cloud snapshot
status: done
priority: high
size: L
points: 8
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
tags: [cloud, ui]
created: 2026-09-02
updated: 2026-09-02T18:07:57Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-56e306a1: Render the shared board from the cloud snapshot

## Description

Replace the taskmark-cloud board stub with shared `StaticBoardApp` fed by the project snapshot, poll version for refresh, and show an empty state that points to Settings.

## Acceptance criteria

- [x] Signed-in members see the hosted board from the stored snapshot using shared components.
- [x] The page refreshes when the board version changes.
- [x] Projects without a snapshot show empty-state copy with Settings and `TASKMARK_SYNC_TOKEN` instructions.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: hosted read-only board that matches local UI and refreshes after sync. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Rendered the hosted board from the stored snapshot with live refresh. |
