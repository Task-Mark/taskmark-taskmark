---
id: T-MM-284fef62
type: task
title: Add /tkmd-version command and skill
status: done
priority: high
size: M
points: 5
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
tags: [plugin, versioning]
created: 2026-08-29
updated: 2026-08-29T17:18:08Z
started_at: 2026-08-29T17:13:00Z
completed_at: 2026-08-29T17:18:08Z
---

# T-MM-284fef62: Add /tkmd-version command and skill

## Description

Add `/tkmd-version`. If Unreleased is empty, run the same collection as changelog or stop if nothing is new. Infer SemVer (breaking → major, new capability → minor, bugs/docs/internal → patch; in `0.x` breaking may stay minor). Explicit version from the user wins. Write the version into the board `package.json`, promote Unreleased to `## {version} - YYYY-MM-DD` (newest first), leave Unreleased empty.

## Acceptance criteria

- [x] `commands/tkmd-version.md` and `skills/tkmd-version/SKILL.md` exist in the plugin package
- [x] Infers or accepts a version and writes it only to the board `package.json`
- [x] Promotes Unreleased into a dated version section and clears Unreleased
- [x] Does not create git tags, GitHub Releases, npm publish, commits, or pushes
- [x] Does not bump plugin.json, marketplace, or `@taskmark/ui`

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
| Marco Mendão | 2026-08-29T17:13:00Z | 2026-08-29T17:14:13Z | Added `/tkmd-version` command and skill. |
