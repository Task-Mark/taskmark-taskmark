---
id: T-048
type: task
title: Build shared work item sheet shell
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-015, T-012]
points: 3
points_source: suggested
estimate_minutes: 50
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

# T-048: Build shared work item sheet shell

## Description

Build a reusable sheet shell for work item detail views using the existing Sheet UI primitive. Include header (id/title/type), scrollable body slot, and close control.

## Acceptance criteria

- [ ] Shared sheet component can host arbitrary detail content in a scrollable body.
- [ ] Header area supports id, title, and optional type/status badges.
- [ ] Sheet can open and close via controlled state.
- [ ] Visual style matches the board UI.

## Notes

Reuse `components/ui/sheet.tsx`. Do not implement type-specific body layouts here.

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
