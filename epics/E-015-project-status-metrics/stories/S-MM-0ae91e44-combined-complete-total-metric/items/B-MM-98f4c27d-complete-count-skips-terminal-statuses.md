---
id: B-MM-98f4c27d
type: bug
title: Complete count ignores terminal statuses besides done
status: done
priority: high
size: M
points: 5
parent: S-MM-0ae91e44
epic: E-015
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
tags: [frontend, metrics, counts]
created: 2026-08-30
updated: 2026-08-30T07:06:06Z
started_at: 2026-08-30T06:57:15Z
completed_at: 2026-08-30T07:06:06Z
---

# B-MM-98f4c27d: Complete count ignores terminal statuses besides done

`aggregateWorkItemCounts` increments complete only when `status === "done"` and drops `cancelled` from both sides. The rest of the board treats `done`, `shelved`, and `cancelled` as complete (`isCompletedStatus`, hide-completed, parent rollup). Shelved leaves therefore inflate total but not complete. Childless stories stay derived `backlog`, so they also keep complete below total even when every task and bug is terminal. Boards where every visible task looks complete can still show two different numbers.

## Fix criteria

- [x] Complete uses the same terminal set as the board lists: `done`, `shelved`, and `cancelled`.
- [x] Total and complete use the same countable set (stories, tasks, bugs; epics excluded) so cancelled items are not missing from one side only.
- [x] When every countable item is terminal, complete equals total.
- [x] Childless stories do not keep the fraction mismatched when every task and bug is terminal (exclude them from both counts, or count only task/bug leaves — pick one rule and apply it to total and complete).
- [x] Tests cover all-done, mixed shelved, cancelled, and childless-story cases.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-30T06:46:00Z | prompt | Marco Mendão | Combine Total and Complete work item cards into one `500/400` Complete work items card; also fix complete counts that stayed below total when every task looked done. |
| 2026-08-30T06:57:15Z | prompt | Marco Mendão | /tkmd-do S-MM-ceafbfa9 e S-MM-0ae91e44 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-30T06:57:15Z | 2026-08-30T07:06:06Z | Count done/shelved/cancelled; drop childless stories from both sides |
