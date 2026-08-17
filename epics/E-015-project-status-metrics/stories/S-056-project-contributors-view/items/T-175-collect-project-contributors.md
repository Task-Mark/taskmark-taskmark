---
id: T-175
type: task
title: Collect unique project contributors
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-120, T-111]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-056
epic: E-015
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
tags: [frontend, contributors, identity]
created: 2026-07-27
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 0
---
# T-175: Collect unique project contributors

## Description

Build a helper that walks loaded work items’ `reporters` and `resolvers`, dedupes by email, and returns a stable sorted list of `ContributorIdentity` for the project overview.

## Acceptance criteria

- [x] Deduplicate by normalized email.
- [x] Prefer non-empty name/initials when merging duplicates.
- [x] Stable sort (name, then email).
- [x] Reuses existing identity types from E-011.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:55:45Z | prompt | Marco Mendão | Create epic for project status metrics (total/complete/speed + contributors) styled like neo-brutalism metric cards; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:27:20Z | 2026-07-27T06:27:20Z | shared-batch: 0 of 3min by points — implement E-015 (T-175) |
