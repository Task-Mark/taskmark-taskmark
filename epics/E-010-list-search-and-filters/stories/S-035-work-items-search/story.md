---
id: S-035
type: story
title: Search on Work items list
status: done
priority: high
size: S
size_source: rolled_up
size_basis: [sum:tasks]
points: 2
points_source: rolled_up
estimate_minutes: 30
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
tags: [dashboard, frontend, search, workitems]
created: 2026-07-23
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 12000
---
# S-035: Search on Work items list

## User story

As a user on the Work items tab, I want to search by code or title across stories and epic-direct tasks/bugs, so the flat list stays findable.

## Acceptance criteria

- [x] Work items list has a search box filtering by id/title.
- [x] Existing sort order is preserved among matches.
- [x] Search resets pagination to page 1.

## Tasks

- [T-100: Search work items list](items/T-100-search-work-items-list.md)

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
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered S-035 |
