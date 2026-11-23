---
id: S-MO-71fe0e31
type: story
title: "/tkmd-shelf command and leaf semantics"
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
tags: [plugin, commands]
created: 2026-08-29
updated: 2026-08-29T10:53:00Z
started_at: null
completed_at: null
---

# S-MO-71fe0e31: /tkmd-shelf command and leaf semantics

## User story

As a Cursor user, I want `/tkmd-shelf` on a task, story, or epic so I can discard work that will never be implemented without marking it done.

## Acceptance criteria

- [ ] The plugin exposes `/tkmd-shelf` (command + skill) and always-apply rules list it with init, plan, do, and commit.
- [ ] A leaf target is written to `status: shelved` with `completed_at` set; parent `epic.md` / `story.md` are not edited.
- [ ] A story or epic target shelves every open, non-cancelled, non-shelved descendant task/bug leaf the same way.
- [ ] `/tkmd-do` treats shelved leaves like cancelled: they are not mandatory remaining scope.
- [ ] The command never commits or pushes.
