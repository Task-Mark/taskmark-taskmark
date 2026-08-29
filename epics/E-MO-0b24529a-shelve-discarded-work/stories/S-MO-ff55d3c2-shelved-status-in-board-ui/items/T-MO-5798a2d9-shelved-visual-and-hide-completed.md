---
id: T-MO-5798a2d9
type: task
title: Distinct shelved chrome and hide-completed
status: done
priority: high
size: M
points: 5
parent: S-MO-ff55d3c2
epic: E-MO-0b24529a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
blocked: false
cancelled: false
tags: [dashboard, frontend, overall]
created: 2026-08-29
updated: 2026-08-29T11:06:17Z
started_at: 2026-08-29T10:58:00Z
completed_at: 2026-08-29T11:03:58Z
---

# T-MO-5798a2d9: Distinct shelved chrome and hide-completed

## Description

Show `shelved` as visually distinct from `done` on Overall, flat work-item lists, and detail. Treat `shelved` as complete for hide-completed, completeness sort, and parent status rollup.

## Acceptance criteria

- [x] Status badge (and row treatment) for `shelved` is distinct from `done` and from `cancelled`.
- [x] Hide-completed hides shelved nodes unless they have a still-visible incomplete descendant.
- [x] `isOverallNodeComplete` (and equivalent list filters) include `shelved`.
- [x] Parent rollup: all leaves `shelved` → `shelved`; all terminal with at least one `done` → `done`.
- [x] Tests cover hide-completed and rollup for shelved.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:53:00Z | prompt | Marco Mendão | New `/tkmd-shelf` to discard never-implemented tasks/epics/stories; distinct from done; hide-completed hides shelved. |
| 2026-08-29T11:03:58Z | prompt | Marco Mendão | Implement E-MO-0b24529a and all open descendant leaves. |
| 2026-08-29T11:06:17Z | feedback | Marco Mendão | Apply necessary follow-up findings from the completed implementation audits. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T10:58:00Z | 2026-08-29T10:59:52Z | Added shelved styling, rollups, filters, sorting, and tests. |
| Marco Mendão | 2026-08-29T11:05:00Z | 2026-08-29T11:05:24Z | Added the distinct shelved row treatment to the task list. |
