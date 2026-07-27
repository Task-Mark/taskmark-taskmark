---
id: T-018
type: task
title: Place board inside project git root
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-003, T-004]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
estimate_basis: [calibrated:T-018]
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
tags: [architecture, single-repo, init]
created: 2026-07-21
updated: 2026-07-27T05:18:44.416Z
started_at: 2026-07-21T22:04:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 60000
---

# T-018: Place board inside project git root

## Description

In single-project mode, ensure `taskmark/` is initialized and maintained only under the project’s git root, and that board commits use that repository (no sibling `-taskmark` project).

## Acceptance criteria

- [x] `taskmark-init` / sync paths create `taskmark/` inside the sole project root.
- [x] No dedicated sibling Taskmark project is created in single-project mode.
- [x] Board file commits are expected against the project’s existing git.

## Notes

Pairs with T-019 for REPOS.md content.

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
| 1 | Marco Mendão | 2026-07-21T22:04:51Z | 2026-07-21T22:05:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 1 of 1min by points |
