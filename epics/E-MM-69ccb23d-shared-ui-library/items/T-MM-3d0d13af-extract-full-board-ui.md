---
id: T-MM-3d0d13af
type: task
title: Extract full board UI into the shared package
status: done
priority: high
size: L
points: 8
parent: E-MM-69ccb23d
epic: E-MM-69ccb23d
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
tags: [ui, board]
created: 2026-09-02
updated: 2026-09-02T18:07:57Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-3d0d13af: Extract full board UI into the shared package

## Description

Move presentational board screens from `@taskmark/ui` into `@taskmark/components/board`, including lists, metrics, the detail sheet, and `StaticBoardApp`, with a data seam that does not import filesystem loaders.

## Acceptance criteria

- [x] Cloud and local can import `StaticBoardApp` from the shared package.
- [x] Shared board components do not import frontend server actions or filesystem loaders.
- [x] The local board still works in live, serve, and static snapshot modes.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: reuse the same board components in cloud and local so UI updates land in both. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Moved presentational board screens into the shared package. |
