---
id: T-115
type: task
title: Stamp resolver on complete-work
status: done
priority: high
size: M
size_source: suggested
size_basis: [velocity:similar]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-040
epic: E-011
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
tags: [identity, plugin, complete-work]
created: 2026-07-23
updated: 2026-07-24T17:39:50.198Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---

# T-115: Stamp resolver on complete-work

## Description

When a work item is completed via `complete-work`, append the current git identity to `resolvers` (merged by email).

## Acceptance criteria

- [x] Completing an item adds current git user to `resolvers`.
- [x] Re-completing / cascade does not duplicate the same email.
- [x] complete-work skill documents resolver stamping.

## Notes

Consider also stamping on start-work for “developed by” provenance if useful; resolver on complete is the required path.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T17:28:57Z | prompt | Marco Mendão | User asked to start developing epic E-011. |
| 2 | 2026-07-23T17:36:57Z | feedback | Marco Mendão | Delivered identity schema, git helper, README sync, list avatars, activity authors. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:29:57Z | 2026-07-23T17:30:57Z | delivered; shared-batch: 1 of 8min by points |
