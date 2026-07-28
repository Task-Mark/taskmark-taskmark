---
id: T-171
type: task
title: Aggregate total and done work item counts
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-067, T-070]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-054
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
tags: [frontend, metrics, counts]
created: 2026-07-27
updated: 2026-07-28T14:32:06.722Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 0
---
# T-171: Aggregate total and done work item counts

## Description

Add a shared helper that, given loaded board items, returns `{ total, complete }` for stories + bugs + tasks only (no epics). Exclude cancelled from both counts.

## Acceptance criteria

- [x] Total = count of story/bug/task where `cancelled` is false.
- [x] Complete = subset with `status: done`.
- [x] Helper is pure / unit-testable from existing board row types.
- [x] Document cancelled exclusion in a short code comment.

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
| 1 | Marco Mendão | 2026-07-27T06:26:20Z | 2026-07-27T06:26:20Z | shared-batch: 0 of 3min by points — implement E-015 (T-171) |
