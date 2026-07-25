---
id: T-098
type: task
title: Search story list
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-092, T-097]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-034
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
tags: [dashboard, frontend, search, stories]
created: 2026-07-23
updated: 2026-07-25T10:44:19.816Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 12000
---
# T-098: Search story list

## Description

Wire shared search into the Overall story list for the selected epic.

## Acceptance criteria

- [x] Search box filters stories by id/title.
- [x] Changing selected epic clears or re-scopes search appropriately (document; prefer keep query, refilter).
- [x] Page resets when query changes.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:03:09Z | prompt | Marco Mendão | implement E-010 list search and filters |
| 2 | 2026-07-23T16:03:09Z | feedback | Marco Mendão | delivered search, parent/tags filters, hide completed |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:01:01Z | shared-batch: 12792 of 140714ms by points; delivered T-098 |
