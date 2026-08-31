---
id: T-MM-db5fb1be
type: task
title: Add the /tkmd-reportme command and skill
status: backlog
priority: high
size: M
points: 5
parent: S-MM-6b6bcec6
epic: E-MM-5a80f20a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, command, reports]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
---

# T-MM-db5fb1be: Add the /tkmd-reportme command and skill

## Description

Add a `commands/tkmd-reportme.md` dispatch file and a `skills/tkmd-reportme/SKILL.md` in the plugin package, mirroring the shape of the existing changelog command. The skill locates the canonical board, reads the board writing language, resolves the cutoff from the newest earlier report filename, keeps only done leaves whose resolvers match the current git identity, and writes a single report file.

Bullets follow the changelog wording rules: past tense, one user-visible outcome each, phrased from the leaf title, user story, or acceptance criteria rather than commit messages, grouped under Keep a Changelog category headings with empty categories omitted. The only write target is `.reports/report-YYYYMMDD.md`.

## Acceptance criteria

- [ ] `/tkmd-reportme` exists as a command and resolves to the matching skill
- [ ] The report file is written at `.reports/report-YYYYMMDD.md`, creating `.reports/` when absent
- [ ] Leaves are filtered to `status: done` with the current git identity in `resolvers`; shelved and cancelled are skipped
- [ ] The cutoff ignores a report already dated today, so same-day re-runs regenerate rather than emptying the report
- [ ] Bullets carry no work-item codes and are written in the board writing language
- [ ] Nothing qualifying still produces a file with a short note
- [ ] The skill states it never commits, pushes, edits item markdown, writes `CHANGELOG.md` or the README, or runs from `/tkmd-do`

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: add a `/tkmd-reportme` command that collects everything I did since the last report and writes it as human-readable bullets like the changelog. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
