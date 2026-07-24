---
id: T-048
type: task
title: Build shared work item sheet shell
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:T-048]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-018
epic: E-005
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
tags: [ui, sheet, frontend]
created: 2026-07-21
updated: 2026-07-24T17:39:50.198Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 18281
---

# T-048: Build shared work item sheet shell

## Description

Build a reusable sheet shell for work item detail views using the existing Sheet UI primitive. Include header (id/title/type), scrollable body slot, and close control.

## Acceptance criteria

- [x] Shared sheet component can host arbitrary detail content in a scrollable body.
- [x] Header area supports id, title, and optional type/status badges.
- [x] Sheet can open and close via controlled state.
- [x] Visual style matches the board UI.

## Notes

Reuse `components/ui/sheet.tsx`. Do not implement type-specific body layouts here.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Marco Mendão | Create all user stories and tasks for E-005 view work item |
| 2 | 2026-07-21T23:56:38Z | feedback | Marco Mendão | Implement E-005 detail sheets delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T23:53:57Z | 2026-07-21T23:54:15.281Z | Delivered as part of E-005; shared-batch: 18281 of 195000ms by points |
