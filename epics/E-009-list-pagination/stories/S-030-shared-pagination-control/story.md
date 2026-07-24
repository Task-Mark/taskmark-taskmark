---
id: S-030
type: story
title: Shared pagination control
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 110
actual_minutes: 2
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-009
epic: E-009
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
tags: [dashboard, frontend, pagination]
created: 2026-07-23
updated: 2026-07-24T17:39:50.198Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 165000
---

# S-030: Shared pagination control

## User story

As a user, I want a reusable pagination bar with first / previous / next / last and a page-size dropdown, so every list can paginate consistently.

## Acceptance criteria

- [x] Shared types/defaults define page index (1-based), page size, and allowed sizes (e.g. 10 / 25 / 50 / 100).
- [x] A reusable UI control shows first, previous, next, last (disabled at bounds) and a page-size select.
- [x] A helper can slice a row array for the current page and report total pages / total count.
- [x] Changing page size resets to page 1 (or clamps to a valid page).

## Tasks

- [T-088: Define pagination types and page-size defaults](items/T-088-pagination-types-defaults.md)
- [T-089: Build pagination navigation and page-size UI](items/T-089-pagination-control-ui.md)
- [T-090: Client-side page slice helper](items/T-090-page-slice-helper.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:29:50Z | prompt | Marco Mendão | Create epic for list pagination with nav + page size; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:35:42Z | shared-batch parent rollup (0 min); leaves hold effort |
