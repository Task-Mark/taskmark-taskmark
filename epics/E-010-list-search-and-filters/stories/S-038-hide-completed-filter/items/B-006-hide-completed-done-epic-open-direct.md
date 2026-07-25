---
id: B-006
type: bug
title: Hide completed hides done epics that still have open epic-direct work
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-103, B-005]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-038
epic: E-010
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
tags: [dashboard, frontend, filters, bug]
created: 2026-07-24
updated: 2026-07-25T10:44:19.816Z
started_at: 2026-07-24T17:38:01Z
completed_at: 2026-07-24T17:38:52Z
actual_ms: 51000
---

# B-006: Hide completed hides done epics that still have open epic-direct work

## Description

After adding a backlog epic-direct task (e.g. T-159) under a previously completed epic (E-005), enabling **Hide completed** removes that epic from the Overall list even though it still has open work. The epic frontmatter can remain `done` (status derived from stories only), and the filter drops `done` rows before consulting child progress.

## Repro steps

1. Complete an epic so all stories are done and epic status is `done`.
2. Create a new epic-direct task/bug under that epic (`epics/E-NNN/items/`) left in `backlog`.
3. On the Overall epic list, enable Hide completed.

## Fix criteria

- [x] With Hide completed on, an epic (or story) whose child progress is incomplete stays visible even if frontmatter status is still `done`.
- [x] Hide completed still hides parents whose children are all done (and leaf rows with status `done`).
- [x] Epic status derivation treats epic-direct tasks/bugs as children (alongside stories) so a done epic reopens when open epic-direct work is added; clear `completed_at` when leaving `done`.
- [x] E-005 is reopened (`in_progress`) while T-159 remains open.

## Notes

- Frontend safety: prefer `workItemCount` / `doneWorkItemCount` over status when progress totals are present.
- Conventions: update status-derivation epic rules to include epic-direct leaves.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:37:37Z | prompt | Marco Mendão | Hide completed hides E-005 despite backlog T-159 under it |
| 2 | 2026-07-24T17:38:52Z | feedback | Marco Mendão | Fixed filter + epic status rules; E-005 reopened |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 80b848a | taskmark-frontend | 2026-07-24T17:40:19Z | Marco Mendão | fix hide-completed for open epic children |
| 55bf8d5 | taskmark-cursor | 2026-07-24T17:40:19Z | Marco Mendão | document reopen parent on new child |
| f6aa2da | taskmark-taskmark | 2026-07-24T17:40:19Z | Marco Mendão | add t-160 and sync board |
| b66202d | taskmark-frontend | 2026-07-25T11:34:33+01:00 | Marco Mendão | add detail sheet routes and overall work items |
| 861fc90 | taskmark-taskmark | 2026-07-25T11:34:33+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T17:38:01Z | 2026-07-24T17:38:52Z | Fixed hide-completed progress preference; reopen E-005; status-derivation epic-direct |
