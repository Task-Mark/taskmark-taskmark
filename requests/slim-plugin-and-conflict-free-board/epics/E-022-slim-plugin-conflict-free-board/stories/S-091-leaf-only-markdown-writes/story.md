---
id: S-091
type: story
title: Only mutate leaf item files on create and do
status: backlog
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 32
points_source: rolled_up
estimate_minutes: 320
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-022
epic: E-022
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, collaboration, board]
created: 2026-08-28
updated: 2026-08-28T12:37:43.783Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-091: Only mutate leaf item files on create and do

## User story

As a teammate, I want agents to change only the markdown of the work they create or finish so that epic.md and story.md stop being constant merge conflicts.

## Acceptance criteria

- [ ] Creating a task writes only the new task file (plus new story/epic files if those are being created).
- [ ] Finishing `/tsmk-do` on task A writes only that task’s MD (status done, AC, work log on that file).
- [ ] Parent Stories/Tasks lists and points/status rollups are queries in the UI (and any generated-only index), not edits to parent files.
- [ ] Parents are not flipped to `in_progress` as a side effect of starting leaf work.
- [ ] Prompt & feedback, Commits and Work log stay on leaves; parent UI shows the aggregated leaf tables without writing parent markdown.
- [ ] Parent displayed status, implementers, and started/updated/completed timestamps are inferred from leaves; only leaf files are mutated for those fields.

## Tasks

- [T-294: Create writes only new item files](items/T-294-create-without-parent-edits.md)
- [T-295: tsmk-do mutates only the implemented leaf markdown](items/T-295-do-mutates-only-target-leaf.md)
- [T-296: Derive parent lists, status, and rollups in the UI](items/T-296-ui-query-parents-and-rollups.md)
- [T-302: Show parent logs, status, people, and dates from leaves](items/T-302-parent-ui-from-leaf-logs-status-people-dates.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:19:14Z | prompt | Marco Mendão | Full housekeeping: slim commands, drop derived board files, static sizing, leaf-only MD, new IDs, delete unused plugin pieces. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
