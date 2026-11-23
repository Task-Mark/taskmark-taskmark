---
id: S-MM-5fb0e29c
type: story
title: Maintainer release script after version
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
tags: [release, npm, git]
created: 2026-09-15
updated: 2026-09-15T16:54:00Z
started_at: null
completed_at: null
---
# S-MM-5fb0e29c: Maintainer release script after version

## Description

After changelog, version, and commit, a maintainer runs one local script that pushes every product repository and publishes the public npm packages. Version numbers are already on disk from `/tkmd-version`; this script does not bump them.

## User story

As a maintainer, I run one release script after `/tkmd-commit` so every repo is pushed and every public npm package is published, including npm login and a 2FA code when needed.

## Acceptance criteria

- [ ] A plugin script pushes every sibling product git root that has a remote.
- [ ] Public npm packages (`@taskmark/components`, then `@taskmark/ui`) are published at the board SemVer.
- [ ] The script logs in to npm when `npm whoami` fails, then asks once for a 2FA code used for publish.
- [ ] The script does not commit, bump versions, or run if working trees are dirty.
