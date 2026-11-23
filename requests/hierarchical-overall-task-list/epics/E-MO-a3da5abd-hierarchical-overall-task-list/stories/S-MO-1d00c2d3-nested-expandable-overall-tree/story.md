---
id: S-MO-1d00c2d3
type: story
title: Nested expandable Overall tree
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

# S-MO-1d00c2d3: Nested expandable Overall tree

## User story

As a board user, I want Overall to show the work hierarchy in one nested list so I can open an epic and then a story and see their children in place instead of jumping between three tables.

## Acceptance criteria

- [ ] Overall is one hierarchical list, not separate epic / work-items / sub-tasks tables stacked on the page.
- [ ] Expanding an epic inserts its stories and epic-direct tasks/bugs directly under that epic.
- [ ] Expanding a story inserts its tasks and bugs directly under that story.
- [ ] Rows keep useful chrome (id, title, type, status, size/points, child progress, attribution, open-detail).
- [ ] Empty board and empty-children states are clear.
- [ ] Opening the work-item sheet does not collapse the tree.
