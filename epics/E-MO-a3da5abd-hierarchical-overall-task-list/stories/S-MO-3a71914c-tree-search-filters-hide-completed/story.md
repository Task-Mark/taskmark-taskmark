---
id: S-MO-3a71914c
type: story
title: Search and filters on the Overall tree
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

# S-MO-3a71914c: Search and filters on the Overall tree

## User story

As a board user, I want search, hide-completed, and timeframe to work on the nested Overall list so I can find work without flattening the hierarchy.

## Acceptance criteria

- [ ] Search matches id/title (and existing searchable fields) at any depth and keeps ancestor rows visible so the match stays in context.
- [ ] Hide-completed hides completed nodes unless they have a visible matching descendant.
- [ ] Timeframe still filters Overall using the existing completion/timeframe rules.
- [ ] All, Stories, and Tasks views are unchanged.
