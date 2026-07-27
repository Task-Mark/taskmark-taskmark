---
id: S-033
type: story
title: Shared search control
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 4
points_source: rolled_up
estimate_minutes: 60
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
tags: [dashboard, frontend, search]
created: 2026-07-23
updated: 2026-07-27T05:16:43.229Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 24000
---
# S-033: Shared search control

## User story

As a user, I want a reusable search box that matches work-item codes or titles, so every list can offer the same find behavior.

## Acceptance criteria

- [x] Shared helpers match a query against item `id` and `title` (case-insensitive; trim; empty query = no filter).
- [x] A reusable search input UI fits board list toolbars (clearable).
- [x] Match behavior is documented for partial id and title substrings.

## Tasks

- [T-095: Define search match helpers and filter types](items/T-095-search-match-helpers.md)
- [T-096: Build shared list search box UI](items/T-096-list-search-box-ui.md)

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
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered S-033 |
