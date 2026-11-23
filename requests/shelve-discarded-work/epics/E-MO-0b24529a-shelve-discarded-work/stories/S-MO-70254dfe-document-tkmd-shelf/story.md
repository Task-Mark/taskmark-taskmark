---
id: S-MO-70254dfe
type: story
title: Document /tkmd-shelf and shelved status
status: backlog
priority: medium
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
tags: [docs, website, commands]
created: 2026-08-29
updated: 2026-08-29T10:53:00Z
started_at: null
completed_at: null
---

# S-MO-70254dfe: Document /tkmd-shelf and shelved status

## User story

As someone reading Taskmark docs, I want `/tkmd-shelf` and `status: shelved` described so I know discarded work is closed, visually distinct from done, and hidden by hide-completed.

## Acceptance criteria

- [ ] Commands/workflows docs include `/tkmd-shelf` (discard, never implemented; never commits).
- [ ] Specification lists `shelved` as a terminal leaf status and notes parent rollup plus hide-completed behaviour.
- [ ] Plugin/README copy that still says “exactly four commands” is updated to include shelf.
