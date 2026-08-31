---
id: S-MM-7ea12eae
type: story
title: Report command docs and plugin sync
status: backlog
priority: medium
size: null
points: null
parent: E-MM-5a80f20a
epic: E-MM-5a80f20a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [docs, plugin, tests]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
---

# S-MM-7ea12eae: Report command docs and plugin sync

## User story

As a maintainer, I want `/tkmd-reportme` documented in the same places as every other Taskmark command and guarded by the plugin test suite, so agents treat it as part of the allowed command set and the local install stays current.

## Acceptance criteria

- [ ] The always-applied rule lists `/tkmd-reportme` in the command allowlist with its write boundary
- [ ] The plugin README and the repository README both document the command
- [ ] Plugin and marketplace descriptions list the current command set instead of a stale subset
- [ ] The plugin test suite covers the new command and skill and passes
- [ ] The local plugin install under `~/.cursor/plugins/local/taskmark` is synced after the package changes
