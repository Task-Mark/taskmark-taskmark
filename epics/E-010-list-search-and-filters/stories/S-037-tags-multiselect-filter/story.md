---
id: S-037
type: story
title: Tags multiselect filter
status: done
priority: medium
size: S
size_source: rolled_up
size_basis: [sum:tasks]
points: 3
points_source: rolled_up
estimate_minutes: 50
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-010
epic: E-010
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
tags: [dashboard, frontend, filters, tags]
created: 2026-07-23
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 19000
---
# S-037: Tags multiselect filter

## User story

As a user, I want to multiselect tags to filter lists, so I can focus on items labeled with those tags.

## Acceptance criteria

- [x] Multiselect shows tags present on the current board’s work items.
- [x] Selecting one or more tags keeps rows that have any (or all — document choice; prefer **any**) of the selected tags.
- [x] Clearing tags removes the filter.
- [x] Available on Work items at minimum; Overall lists if tags are already on those rows.

## Tasks

- [T-102: Tags multiselect filter](items/T-102-tags-multiselect-filter.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:53:02Z | prompt | Marco Mendão | Epic for list search + parent/tag filters + hide completed; create stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered S-037 |
