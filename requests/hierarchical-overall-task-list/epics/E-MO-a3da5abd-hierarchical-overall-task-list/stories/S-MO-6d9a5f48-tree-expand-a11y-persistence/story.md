---
id: S-MO-6d9a5f48
type: story
title: Expand, keyboard, and persistence
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

# S-MO-6d9a5f48: Expand, keyboard, and persistence

## User story

As a board user, I want expand/collapse to be obvious, keyboard-accessible, and sticky so I can move through the hierarchy without fighting the UI.

## Acceptance criteria

- [ ] Chevron/row expand is distinct from opening the work-item sheet.
- [ ] Expanded node ids persist for the session (refresh does not wipe them unexpectedly).
- [ ] Keyboard: expand/collapse with Enter/Space; optional arrow navigation.
- [ ] Expand controls expose `aria-expanded` (and a tree or treegrid pattern where practical).
- [ ] Indent and hit targets work on a typical mobile viewport.
