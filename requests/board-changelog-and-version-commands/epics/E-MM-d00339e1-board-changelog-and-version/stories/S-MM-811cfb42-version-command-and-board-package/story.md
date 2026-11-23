---
id: S-MM-811cfb42
type: story
title: /tkmd-version and board package version
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
tags: [versioning, plugin]
created: 2026-08-29
updated: 2026-08-29T16:56:10Z
started_at: null
completed_at: null
---

# S-MM-811cfb42: /tkmd-version and board package version

## User story

As a maintainer, I want `/tkmd-version` to infer (or accept) a SemVer, move Unreleased notes under that version, and set the board `package.json` version so the release number lives in one place.

## Acceptance criteria

- [ ] The board `package.json` has a `version` field
- [ ] `/tkmd-version` exists as a Cursor command and skill
- [ ] It infers major/minor/patch from Unreleased work, or uses an explicit version
- [ ] It promotes Unreleased into `## x.y.z - YYYY-MM-DD`, clears Unreleased, and does not commit, tag, or publish
