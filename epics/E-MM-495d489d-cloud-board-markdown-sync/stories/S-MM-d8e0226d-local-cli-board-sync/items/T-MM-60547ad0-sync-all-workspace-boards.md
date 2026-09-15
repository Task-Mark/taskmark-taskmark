---
id: T-MM-60547ad0
type: task
title: Sync every configured workspace board in the background
status: done
priority: high
size: M
points: 5
parent: S-MM-d8e0226d
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
tags: [cli, sync, workspace]
created: 2026-09-15
updated: 2026-09-15T17:21:01Z
started_at: 2026-09-15T17:16:22Z
completed_at: 2026-09-15T17:21:01Z
---
# T-MM-60547ad0: Sync every configured workspace board in the background

## Description

Extend standalone workspace mode so `npx @taskmark/ui` starts Cloud synchronization for every discovered project configured in that UI instance, rather than synchronizing only the currently selected board. Each board with valid Cloud credentials in its root `.config` must push once and keep watching markdown and configuration changes in the background.

## User story

As a developer using the standalone multi-project UI, I want every configured local board to keep synchronizing with Taskmark Cloud so updates reach Cloud without opening each project individually.

## Acceptance criteria

- [x] Standalone workspace mode starts background Cloud sync for every discovered board whose `.config` contains a valid token.
- [x] All configured boards remain watched regardless of which project is currently selected in the UI.
- [x] Reconciliation avoids duplicate watchers and stops watchers for projects removed from the configured workspace.
- [x] Existing bound `dev` and `serve` synchronization continues without duplicate workspace watchers.
- [x] Automated tests cover multi-board startup, deduplication, and watcher cleanup.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T17:16:22Z | prompt | Marco Mendão | Make `npx @taskmark/ui` continuously push every configured project with Cloud settings in `.config`, in the background and independently of the project currently open. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T17:16:22Z | 2026-09-15T17:21:01Z | Added non-blocking multi-board workspace sync reconciliation, cleanup, and automated coverage while preserving bound-mode sync. |
