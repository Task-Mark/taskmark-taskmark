---
id: B-016
type: bug
title: "taskmark dev from product repo misses sibling *-taskmark board"
status: backlog
priority: high
size: S
size_source: suggested
size_basis: [T-150]
points: 2
points_source: suggested
estimate_minutes: 28
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: E-014
epic: E-014
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cli, board-resolution, multi-repo]
created: 2026-08-10
updated: 2026-08-10T16:02:29Z
started_at: 2026-08-10T16:02:29Z
completed_at: null
---

# B-016: taskmark dev from product repo misses sibling *-taskmark board

## Description

In a multi-git workspace, running `yarn dev` / `taskmark dev` from a product repo (e.g. `taskmark-frontend`) fails with “No Taskmark board found” even though the dedicated sibling board (`taskmark-taskmark`) sits next to it. Cwd resolution only checks nested `./taskmark/` or cwd itself being `*-taskmark`.

## Repro steps

1. `cd taskmark-frontend` in the Taskmark multi-repo workspace.
2. `yarn dev` (or `taskmark dev`).
3. Error: No Taskmark board found.

## Fix criteria

- [x] From a product repo cwd, resolve sibling `<parentBasename>-taskmark` (or a unique `*-taskmark` sibling) when env/flags are unset.
- [x] CLI help documents sibling discovery.
- [x] `yarn dev` from `taskmark-frontend` binds to `taskmark-taskmark`.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-10T16:02:29Z | prompt | Marco Mendão | yarn dev from taskmark-frontend: no board found |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| bd7d5b4 | taskmark-frontend | 2026-08-10T17:04:19+01:00 | Marco Mendão | resolve sibling taskmark board from product cwd |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-10T16:02:29Z | — | In progress: sibling *-taskmark board resolution |
