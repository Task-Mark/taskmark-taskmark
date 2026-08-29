---
id: T-MM-167fb33f
type: task
title: Add version field to board package.json
status: done
priority: high
size: XS
points: 1
parent: S-MM-811cfb42
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [versioning]
created: 2026-08-29
updated: 2026-08-29T17:18:08Z
started_at: 2026-08-29T17:13:00Z
completed_at: 2026-08-29T17:18:08Z
---

# T-MM-167fb33f: Add version field to board package.json

## Description

`taskmark-taskmark/package.json` has no `version`. Add a starting SemVer (for example `0.1.0`) so `/tkmd-version` has a canonical field to bump. Do not change plugin or `@taskmark/ui` versions.

## Acceptance criteria

- [x] Board `package.json` includes a valid SemVer `version`
- [x] Plugin `plugin.json`, marketplace metadata, and `@taskmark/ui` versions are unchanged

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T16:56:10Z | prompt | Marco Mendão | `/tkmd-save`: Cursor plan for `/tkmd-changelog` and `/tkmd-version` with CHANGELOG.md on the board and version on taskmark-taskmark package.json. |
| 2026-08-29T17:13:00Z | prompt | Marco Mendão | `/tkmd-do`: implement every open descendant of epic E-MM-d00339e1. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T17:13:00Z | 2026-08-29T17:13:14Z | Added SemVer to the board package.json. |
