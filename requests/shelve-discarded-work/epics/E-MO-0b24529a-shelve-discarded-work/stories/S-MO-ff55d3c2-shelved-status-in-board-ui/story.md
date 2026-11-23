---
id: S-MO-ff55d3c2
type: story
title: Shelved items look distinct and hide with completed
status: backlog
priority: high
size: null
points: null
parent: E-MO-0b24529a
epic: E-MO-0b24529a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, overall]
created: 2026-08-29
updated: 2026-08-29T10:53:00Z
started_at: null
completed_at: null
---

# S-MO-ff55d3c2: Shelved items look distinct and hide with completed

## User story

As a board user, I want shelved work to look different from done, and I want hide-completed to drop it so discarded items do not clutter the active list.

## Acceptance criteria

- [ ] Overall tree, flat lists, and detail show `shelved` with a distinct badge/row treatment from `done`.
- [ ] Hide-completed hides shelved nodes (and shelved parents with no remaining visible descendants) the same way it hides done/cancelled.
- [ ] Parent read-time status: all-shelved descendants → `shelved`; mix of done and shelved/cancelled with no open work → `done`.
- [ ] Completeness sort treats `shelved` as complete (after incomplete work).
