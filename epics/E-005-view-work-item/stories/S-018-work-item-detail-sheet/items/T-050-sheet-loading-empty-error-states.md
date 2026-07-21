---
id: T-050
type: task
title: Sheet loading empty and error states
status: backlog
priority: medium
size: S
size_source: suggested
size_basis: [T-015, T-012]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-018
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [ui, sheet, frontend]
created: 2026-07-21
updated: 2026-07-21T23:50:12Z
started_at: null
completed_at: null
---

# T-050: Sheet loading empty and error states

## Description

Add loading, empty/sparse-content, and error presentations inside the work item sheet so failed or incomplete loads remain usable.

## Acceptance criteria

- [ ] Sheet shows a loading state while detail content is fetched.
- [ ] Sheet shows a clear error state when detail cannot be loaded.
- [ ] Sparse items still render available fields without crashing.
- [ ] Error state includes enough context to identify the failed item (id/path/message).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Create all user stories and tasks for E-005 view work item |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
