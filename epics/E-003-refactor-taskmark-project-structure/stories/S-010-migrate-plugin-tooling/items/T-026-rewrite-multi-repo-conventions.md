---
id: T-026
type: task
title: Rewrite multi-repo conventions and rule
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-023, T-005]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 1
estimate_basis: [calibrated:T-026]
session_cap_minutes: 480
parent: S-010
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
tags: [plugin, conventions, docs]
created: 2026-07-21
updated: 2026-07-27T07:06:27.645Z
started_at: 2026-07-21T21:48:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 60000
---
# T-026: Rewrite multi-repo conventions and rule

## Description

Update `multi-repo.md`, related convention refs, and the always-apply Taskmark project-memory rule so they describe single-in-project vs dedicated `<name>-taskmark` git project — not per-repo board copies.

## Acceptance criteria

- [x] Convention docs match the new layout model end-to-end.
- [x] Always-apply rule no longer requires copying `taskmark/` into every git project.
- [x] Examples in docs show both single and multi layouts.

## Notes

Source of truth in `taskmark-cursor/plugins/taskmark`; sync local plugin after.

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
| 1 | Marco Mendão | 2026-07-21T21:48:51Z | 2026-07-21T21:49:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 1 of 2min by points |
