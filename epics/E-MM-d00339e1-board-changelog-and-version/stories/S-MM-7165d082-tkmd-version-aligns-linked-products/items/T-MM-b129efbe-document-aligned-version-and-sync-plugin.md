---
id: T-MM-b129efbe
type: task
title: Document aligned version bump and sync the plugin
status: done
priority: high
size: S
points: 3
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
tags: [docs, plugin, versioning]
created: 2026-08-29
updated: 2026-08-29T20:06:53Z
started_at: 2026-08-29T19:25:00Z
completed_at: 2026-08-29T20:06:53Z
---

# T-MM-b129efbe: Document aligned version bump and sync the plugin

## Description

Update conventions, the always-apply memory rule, plugin and board READMEs, and website command docs so they no longer say `/tkmd-version` writes only the board `package.json` or that it must not bump `plugin.json` / `@taskmark/ui`. State that the chosen SemVer is applied to every linked product. Sync the local Cursor plugin install after the plugin package changes.

## Acceptance criteria

- [x] `taskmark-conventions` and project-memory rules describe the multi-product version write
- [x] Plugin README, board/project README command table, and website `/docs/commands` (plus setup/overview if they name the old behaviour) match
- [x] Local plugin install contains the updated `/tkmd-version` skill and command

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
| Marco Mendão | 2026-08-29T19:25:00Z | 2026-08-29T20:06:53Z | Documented the aligned bump in conventions, READMEs, and website docs; copied the updated skill and command into the local plugin install. |
