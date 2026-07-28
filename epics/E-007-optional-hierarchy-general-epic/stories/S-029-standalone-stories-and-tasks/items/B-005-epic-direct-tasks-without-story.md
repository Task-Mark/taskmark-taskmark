---
id: B-005
type: bug
title: Tasks and bugs cannot live under an epic without a story
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:B-005]
points: 2
points_source: suggested
estimate_minutes: 35
actual_minutes: 36
estimate_source: suggested
estimate_basis: [calibrated:B-005]
session_cap_minutes: 480
parent: S-029
epic: E-007
owner: ""
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
tags: [plugin, hierarchy, bug]
created: 2026-07-23
updated: 2026-07-28T15:03:07.151Z
started_at: 2026-07-23T05:07:15Z
completed_at: 2026-07-23T05:10:15Z
actual_ms: 2186000
---
# B-005: Tasks and bugs cannot live under an epic without a story

## Description

S-029 still forced orphan tasks into General → Unattached. Tasks and bugs should also live directly under any epic at `epics/{E-NNN}/items/` with `parent` = epic id and no story required.

## Repro steps

1. Create a task naming only an epic (no story).
2. Observe it is forced under Unattached or blocked.

## Fix criteria

- [x] Folder layout allows `epics/{E-NNN}-{slug}/items/` for tasks/bugs.
- [x] Frontmatter: `parent` may be an epic id; `epic` set to that epic.
- [x] `create-task` soft-attach prefers story when clear, else epic `items/`, else General epic `items/`.
- [x] Dashboard shows epic-direct tasks when an epic is selected (no story required).
- [x] Recompute rolls epic-direct leaves into the epic.

## Notes

Unattached catch-all story removed; story-less tasks/bugs use epic-level `items/` only (or General).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T05:07:15Z | prompt | Marco Mendão | Fix: tasks/bugs can exist inside an epic without a user story |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9c0c269 | taskmark-cursor | 2026-07-23T05:40:41Z | Marco Mendão | fix epic-direct points rollup |
| dbb8838 | taskmark-cursor | 2026-07-23T05:20:13Z | Marco Mendão | epic-direct tasks drop unattached story |
| cd914a9 | taskmark-frontend | 2026-07-23T05:20:13Z | Marco Mendão | show general tasks under epics |
| 6aae4fd | taskmark-taskmark | 2026-07-23T05:20:14Z | Marco Mendão | remove unattached story fix b-005 |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T05:07:15Z | 2026-07-23T05:10:15Z | Epic-direct items under epics/E/items/; create-task + UI + ensure-general |
| 2 | Marco Mendão | 2026-07-23T05:07:15Z | 2026-07-23T05:40:41Z | auto-recovered: commit span |
