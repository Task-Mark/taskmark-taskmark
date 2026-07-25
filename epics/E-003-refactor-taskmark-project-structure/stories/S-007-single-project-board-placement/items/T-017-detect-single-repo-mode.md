---
id: T-017
type: task
title: Detect single-repo workspace mode
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-008, T-003]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
estimate_basis: [calibrated:T-017]
session_cap_minutes: 480
parent: S-007
epic: E-003
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
tags: [architecture, single-repo, detection]
created: 2026-07-21
updated: 2026-07-25T10:44:19.816Z
started_at: 2026-07-21T22:04:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 60000
---

# T-017: Detect single-repo workspace mode

## Description

Define and implement detection for single-project mode: exactly one workspace folder that is a git root (or one active git root). Document edge cases (nested `.git`, multi-root with one git, etc.).

## Acceptance criteria

- [x] Clear rule: one git root → single-project mode.
- [x] Detection is usable by init/sync skills and any helper script.
- [x] Edge cases documented (when to treat as multi vs single).

## Notes

Feeds S-007 placement and S-008 branching.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for Taskmark project structure refactor |
| 2 | 2026-07-21T22:36:37Z | feedback | Marco Mendão | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:04:51Z | 2026-07-21T22:05:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 1 of 2min by points |
