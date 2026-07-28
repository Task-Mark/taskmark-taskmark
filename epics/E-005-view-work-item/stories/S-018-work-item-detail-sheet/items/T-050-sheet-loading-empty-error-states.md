---
id: T-050
type: task
title: Sheet loading empty and error states
status: done
priority: medium
size: S
size_source: suggested
size_basis: [calibrated:T-050]
points: 2
points_source: suggested
estimate_minutes: 30
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
updated: 2026-07-28T15:03:07.151Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 12188
---

# T-050: Sheet loading empty and error states

## Description

Add loading, empty/sparse-content, and error presentations inside the work item sheet so failed or incomplete loads remain usable.

## Acceptance criteria

- [x] Sheet shows a loading state while detail content is fetched.
- [x] Sheet shows a clear error state when detail cannot be loaded.
- [x] Sparse items still render available fields without crashing.
- [x] Error state includes enough context to identify the failed item (id/path/message).

## Notes

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
| 1 | Marco Mendão | 2026-07-21T23:53:57Z | 2026-07-21T23:54:09.188Z | Delivered as part of E-005; shared-batch: 12188 of 195000ms by points |
