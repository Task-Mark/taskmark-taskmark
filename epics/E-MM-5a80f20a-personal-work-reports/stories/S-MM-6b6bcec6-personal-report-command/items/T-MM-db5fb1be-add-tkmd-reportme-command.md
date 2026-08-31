---
id: T-MM-db5fb1be
type: task
title: Add the /tkmd-reportme command and skill
status: done
priority: high
size: M
points: 5
parent: S-MM-6b6bcec6
epic: E-MM-5a80f20a
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
tags: [plugin, command, reports]
created: 2026-08-31
updated: 2026-08-31T07:09:31Z
started_at: 2026-08-31T06:55:00Z
completed_at: 2026-08-31T07:09:31Z
---

# T-MM-db5fb1be: Add the /tkmd-reportme command and skill

## Description

Add a `commands/tkmd-reportme.md` dispatch file and a `skills/tkmd-reportme/SKILL.md` in the plugin package, mirroring the shape of the existing changelog command. The skill locates the canonical board, reads the board writing language, resolves the cutoff from the newest earlier report filename, keeps only done leaves whose resolvers match the current git identity, and writes a single report file.

Bullets follow the changelog wording rules: past tense, one user-visible outcome each, phrased from the leaf title, user story, or acceptance criteria rather than commit messages, grouped under Keep a Changelog category headings with empty categories omitted. The only write target is `.reports/report-YYYYMMDD.md`.

## Acceptance criteria

- [x] `/tkmd-reportme` exists as a command and resolves to the matching skill
- [x] The report file is written at `.reports/report-YYYYMMDD.md`, creating `.reports/` when absent
- [x] Leaves are filtered to `status: done` with the current git identity in `resolvers`; shelved and cancelled are skipped
- [x] The cutoff ignores a report already dated today, so same-day re-runs regenerate rather than emptying the report
- [x] Bullets carry no work-item codes and are written in the board writing language
- [x] Nothing qualifying still produces a file with a short note
- [x] The skill states it never commits, pushes, edits item markdown, writes `CHANGELOG.md` or the README, or runs from `/tkmd-do`

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: add a `/tkmd-reportme` command that collects everything I did since the last report and writes it as human-readable bullets like the changelog. |
| 2026-08-31T06:55:00Z | prompt | Marco Mendão | /tkmd-do E-MM-5a80f20a |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T06:55:00Z | 2026-08-31T06:59:00Z | Added the command dispatch file and the report skill with cutoff, identity filter, wording rules, and write boundaries. |
