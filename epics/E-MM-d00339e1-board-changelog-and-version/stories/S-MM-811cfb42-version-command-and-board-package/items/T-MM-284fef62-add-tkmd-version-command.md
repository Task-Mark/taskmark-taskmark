---
id: T-MM-284fef62
type: task
title: Add /tkmd-version command and skill
status: backlog
priority: high
size: M
points: 5
parent: S-MM-811cfb42
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, versioning]
created: 2026-08-29
updated: 2026-08-29T16:56:10Z
started_at: null
completed_at: null
---

# T-MM-284fef62: Add /tkmd-version command and skill

## Description

Add `/tkmd-version`. If Unreleased is empty, run the same collection as changelog or stop if nothing is new. Infer SemVer (breaking → major, new capability → minor, bugs/docs/internal → patch; in `0.x` breaking may stay minor). Explicit version from the user wins. Write the version into the board `package.json`, promote Unreleased to `## {version} - YYYY-MM-DD` (newest first), leave Unreleased empty.

## Acceptance criteria

- [ ] `commands/tkmd-version.md` and `skills/tkmd-version/SKILL.md` exist in the plugin package
- [ ] Infers or accepts a version and writes it only to the board `package.json`
- [ ] Promotes Unreleased into a dated version section and clears Unreleased
- [ ] Does not create git tags, GitHub Releases, npm publish, commits, or pushes
- [ ] Does not bump plugin.json, marketplace, or `@taskmark/ui`

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
