---
id: T-MM-2e485e42
type: task
title: Export portable BoardSnapshot types with relative paths
status: done
priority: high
size: M
points: 5
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
tags: [ui, snapshot]
created: 2026-09-02
updated: 2026-09-02T18:07:57Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-2e485e42: Export portable BoardSnapshot types with relative paths

## Description

Move BoardSnapshot and related types into `@taskmark/components/board-model` and make snapshot path keys relative to the board root so a remote client can render them.

## Acceptance criteria

- [x] Snapshot types live in the shared package with no filesystem or React imports.
- [x] `buildBoardSnapshot` stores relative `filePath` keys in `detailsByPath` and `refsById`.
- [x] The local frontend type-checks against the shared types.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: share BoardSnapshot types and normalize relative paths so cloud and local can reuse the same contract. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Exported BoardSnapshot types and relative snapshot paths. |
