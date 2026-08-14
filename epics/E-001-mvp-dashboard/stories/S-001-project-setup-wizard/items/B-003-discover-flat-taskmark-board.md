---
id: B-003
type: bug
title: Setup fails to discover flat multi-repo board
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-008, B-002]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 32
estimate_basis: [calibrated:B-003]
session_cap_minutes: 480
parent: S-001
epic: E-001
owner: ""
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
tags: [setup, discovery, multi-repo, frontend]
created: 2026-07-21
updated: 2026-08-14T17:50:46.835Z
started_at: 2026-07-21T22:44:32Z
completed_at: 2026-07-21T22:44:56Z
actual_ms: 1920000
---

# B-003: Setup fails to discover flat multi-repo board

## Description

After E-003, multi-git boards live at `<common>-taskmark/` root (no nested `taskmark/`). Setup still only looks for `*/taskmark/` boards, so a master folder with only a flat `*-taskmark` project shows "No Taskmark projects found…".

## Repro steps

1. Master folder contains `taskmark-frontend`, `taskmark-cursor`, and flat `taskmark-taskmark/` (INDEX.md at root).
2. Open setup and select that master folder.
3. See error: No Taskmark projects found in subfolders…

## Fix criteria

- [x] Discovery recognizes dedicated `*-taskmark` folders with `INDEX.md` or `epics/` at the repo root.
- [x] Nested `<project>/taskmark/` boards still discover correctly (single-project).
- [x] Setup error copy mentions both layouts.
- [x] Selecting the master folder succeeds when a flat board is present.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:44:32Z | prompt | Marco Mendão | Multi-folder setup shows no projects; flat *-taskmark board not discovered |
| 2 | 2026-07-21T22:44:56Z | feedback | Marco Mendão | discovery fix delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 292c94b | taskmark-frontend | 2026-07-21T22:46:18Z | Marco Mendão | fix discovery for flat taskmark boards |
| 95a7951 | taskmark-taskmark | 2026-07-21T22:46:18Z | Marco Mendão | add b-003 flat board discovery bug |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:12:56Z | 2026-07-21T22:44:56Z | auto-backfilled: velocity × points (missing work log) |
