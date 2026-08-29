---
id: T-MM-4d253142
type: task
title: Add /tkmd-changelog command and skill
status: done
priority: high
size: M
points: 5
parent: S-MM-eadee247
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
tags: [plugin, changelog]
created: 2026-08-29
updated: 2026-08-29T17:18:08Z
started_at: 2026-08-29T17:13:00Z
completed_at: 2026-08-29T17:18:08Z
---

# T-MM-4d253142: Add /tkmd-changelog command and skill

## Description

Add an agent-driven `/tkmd-changelog` command and skill. Rebuild the Unreleased section of board-root `CHANGELOG.md` from done task/bug leaves since the newest `## x.y.z` heading (all done leaves if none). Portuguese Keep a Changelog style. Create the file if missing.

## Acceptance criteria

- [x] `commands/tkmd-changelog.md` and `skills/tkmd-changelog/SKILL.md` exist in the plugin package
- [x] Skill locates the board, writes only `CHANGELOG.md`, and never the README
- [x] Cutoff is the latest released section date; ignores shelved and cancelled leaves
- [x] Unreleased is rewritten idempotently; bullets are user-facing past tense with no T-/B-/S-/E- codes
- [x] Skill never edits epic/story/leaf files, never commits or pushes, never runs from `/tkmd-do`

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
| Marco Mendão | 2026-08-29T17:13:00Z | 2026-08-29T17:14:13Z | Added `/tkmd-changelog` command and skill. |
