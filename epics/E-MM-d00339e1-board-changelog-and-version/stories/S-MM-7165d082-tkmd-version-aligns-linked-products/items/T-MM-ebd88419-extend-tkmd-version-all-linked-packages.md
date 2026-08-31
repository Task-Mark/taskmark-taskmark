---
id: T-MM-ebd88419
type: task
title: Extend /tkmd-version to bump every linked product
status: done
priority: high
size: M
points: 5
parent: S-MM-7165d082
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
tags: [versioning, plugin]
created: 2026-08-29
updated: 2026-08-29T20:06:53Z
started_at: 2026-08-29T19:25:00Z
completed_at: 2026-08-29T20:06:53Z
---

# T-MM-ebd88419: Extend /tkmd-version to bump every linked product

## Description

Change `/tkmd-version` so the SemVer written on the board `package.json` is also written to every other linked system product. Discover roots from local `REPOS.md` (or the same git-root discovery used for linked repos). Set each product-root `package.json` `version` when that file exists. For the Cursor plugin product, set `.cursor-plugin/plugin.json` `version` on the plugin package (not example stubs). Do not bump nested example `package.json` files. Canonical bump still starts from the board `package.json`. Still never commit, tag, or publish.

## Acceptance criteria

- [x] `skills/tkmd-version/SKILL.md` and `commands/tkmd-version.md` require the chosen SemVer on every linked product-root `package.json` that has a version field
- [x] The Cursor plugin `plugin.json` version is set to the same SemVer
- [x] Example/stub packages and README files are not versioned by this command
- [x] The command still does not create tags, GitHub Releases, npm publishes, commits, or pushes

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T19:25:00Z | prompt | Marco Mendão | When `/tkmd-version` runs, the version placed on the Taskmark board must be the version every system project gets; all projects bump together. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T19:25:00Z | 2026-08-29T20:06:53Z | Extended `/tkmd-version` skill and command to write the chosen SemVer to every linked product-root package.json and the Cursor plugin.json. |
