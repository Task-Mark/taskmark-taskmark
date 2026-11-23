---
id: S-MO-bb8f7f8b
type: story
title: Sort Overall incomplete then newest
status: backlog
priority: high
size: null
points: null
parent: E-MO-a3da5abd
epic: E-MO-a3da5abd
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, overall]
created: 2026-08-29
updated: 2026-08-28T23:03:00Z
started_at: null
completed_at: null
---

# S-MO-bb8f7f8b: Sort Overall incomplete then newest

## User story

As a board user, I want Overall ordered so unfinished work comes first and newer items come first so I see what still needs attention before completed history.

## Acceptance criteria

- [ ] At every level (epics, children of an epic, children of a story), incomplete items appear before complete items.
- [ ] Within incomplete and within complete, items sort by recency descending (`created`, newest first; `updated` as tiebreaker).
- [ ] Cancelled items sort with complete (after incomplete).
- [ ] This default order is the Overall tree order; it is not overridden by the old per-table column sort.
