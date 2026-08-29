---
id: S-MM-eadee247
type: story
title: Human-readable CHANGELOG and /tkmd-changelog
status: backlog
priority: high
size: null
points: null
parent: E-MM-d00339e1
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [changelog, plugin]
created: 2026-08-29
updated: 2026-08-29T16:56:10Z
started_at: null
completed_at: null
---

# S-MM-eadee247: Human-readable CHANGELOG and /tkmd-changelog

## User story

As a maintainer, I want `/tkmd-changelog` to rebuild the Unreleased section from recent done leaves in plain language so I can see what shipped without decoding board IDs.

## Acceptance criteria

- [ ] `/tkmd-changelog` exists as a Cursor command and skill
- [ ] It writes `CHANGELOG.md` at the board root (create if missing), never the board README
- [ ] Unreleased bullets are user-facing, past tense, and contain no work-item IDs
- [ ] It does not edit epic/story/leaf markdown, commit, or push
