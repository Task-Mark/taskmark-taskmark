---
id: S-MM-7165d082
type: story
title: /tkmd-version aligns all linked product versions
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
tags: [versioning, plugin, multi-repo]
created: 2026-08-29
updated: 2026-08-29T19:25:00Z
started_at: null
completed_at: null
---

# S-MM-7165d082: /tkmd-version aligns all linked product versions

## User story

As a maintainer, I want `/tkmd-version` to write the same SemVer it puts on the Taskmark board into every linked system product, so a release bump stays consistent across the board, UI, website, and Cursor plugin without hand-editing each package.

## Acceptance criteria

- [ ] `/tkmd-version` still infers or accepts a SemVer, promotes Unreleased, and never commits, tags, or publishes
- [ ] The chosen version is written to every linked product root that has a versioned `package.json`
- [ ] The Cursor plugin package version is set to the same SemVer
- [ ] Conventions, command copy, and public docs describe this aligned bump
