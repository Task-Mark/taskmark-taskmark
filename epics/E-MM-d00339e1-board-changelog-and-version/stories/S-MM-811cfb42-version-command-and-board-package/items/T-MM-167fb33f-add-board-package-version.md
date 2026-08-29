---
id: T-MM-167fb33f
type: task
title: Add version field to board package.json
status: backlog
priority: high
size: XS
points: 1
parent: S-MM-811cfb42
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [versioning]
created: 2026-08-29
updated: 2026-08-29T16:56:10Z
started_at: null
completed_at: null
---

# T-MM-167fb33f: Add version field to board package.json

## Description

`taskmark-taskmark/package.json` has no `version`. Add a starting SemVer (for example `0.1.0`) so `/tkmd-version` has a canonical field to bump. Do not change plugin or `@taskmark/ui` versions.

## Acceptance criteria

- [ ] Board `package.json` includes a valid SemVer `version`
- [ ] Plugin `plugin.json`, marketplace metadata, and `@taskmark/ui` versions are unchanged

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T16:56:10Z | prompt | Marco Mendão | `/tkmd-save`: Cursor plan for `/tkmd-changelog` and `/tkmd-version` with CHANGELOG.md on the board and version on taskmark-taskmark package.json. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
