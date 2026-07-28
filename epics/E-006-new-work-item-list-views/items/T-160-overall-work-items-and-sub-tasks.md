---
id: T-160
type: task
title: Remake Overall work items and sub tasks lists
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-081, T-082, T-066]
points: 3
points_source: suggested
estimate_minutes: 45
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: E-006
epic: E-006
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
tags: [dashboard, frontend, views, overall, workitems]
created: 2026-07-24
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-24T17:41:23Z
completed_at: 2026-07-24T17:42:47Z
actual_ms: 84000
---

# T-160: Remake Overall work items and sub tasks lists

## Description

On the Overall drill-down, remake the post-epic lists:

1. Rename the **Stories** list to **Work items**.
2. That list shows **all** work items under the selected epic — stories, tasks, bugs (including epic-direct leaves), not stories only.
3. When the user selects a **story** from that list, show the child list renamed from **Tasks** to **Sub Tasks** (tasks/bugs under that story).

## Acceptance criteria

- [x] After selecting an epic in Overall, the middle list is labeled **Work items** (not Stories).
- [x] Work items under an epic includes stories, epic-direct tasks/bugs, and any other non-epic children of the epic.
- [x] Selecting a story opens the child list labeled **Sub Tasks** (not Tasks).
- [x] Selecting a non-story work item does not open a Sub Tasks list (or behaves consistently with no children).
- [x] Existing Overall filters, pagination, search, and detail-sheet open still work on these lists.

## Notes

Builds on S-025 / T-082 Overall drill-down; naming aligns with the Work items tab language.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:39:11Z | prompt | Marco Mendão | Remake Overall: Stories→Work items (all epic children); Tasks→Sub Tasks when story selected |
| 2 | 2026-07-24T17:41:23Z | prompt | Marco Mendão | implement T-160 |
| 3 | 2026-07-24T17:42:47Z | feedback | Marco Mendão | Implemented Overall work items + sub tasks lists |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| f6aa2da | taskmark-taskmark | 2026-07-24T17:40:19Z | Marco Mendão | add t-160 and sync board |
| b66202d | taskmark-frontend | 2026-07-25T11:34:33+01:00 | Marco Mendão | add detail sheet routes and overall work items |
| 861fc90 | taskmark-taskmark | 2026-07-25T11:34:33+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T17:41:23Z | 2026-07-24T17:42:47Z | Overall Work items list (stories+epic-direct); Sub Tasks on story select |
