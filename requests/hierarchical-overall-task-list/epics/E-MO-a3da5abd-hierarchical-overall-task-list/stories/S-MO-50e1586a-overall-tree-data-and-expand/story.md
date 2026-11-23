---
id: S-MO-50e1586a
type: story
title: Overall tree data and in-place expand
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

# S-MO-50e1586a: Overall tree data and in-place expand

## User story

As a board user, I want expanding a row to reveal children in place from a full hierarchy model so I do not have to select an epic, scroll to another table, then select a story.

## Acceptance criteria

- [ ] The frontend can build a nested Overall tree from the board (epic → stories and epic-direct leaves → story leaves).
- [ ] Expand happens in the same list, not by rendering a second or third table below.
- [ ] `?epic=` and `?story=` still expand the matching nodes (deep link).
- [ ] Static board Overall uses the same tree.
- [ ] Pagination, if present, pages root epics; children travel with their epic.
