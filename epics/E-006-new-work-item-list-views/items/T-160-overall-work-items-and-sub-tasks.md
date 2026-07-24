---
id: T-160
type: task
title: Remake Overall work items and sub tasks lists
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-081, T-082, T-066]
points: 3
points_source: suggested
estimate_minutes: 45
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, views, overall, workitems]
created: 2026-07-24
updated: 2026-07-24T17:39:50.198Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-160: Remake Overall work items and sub tasks lists

## Description

On the Overall drill-down, remake the post-epic lists:

1. Rename the **Stories** list to **Work items**.
2. That list shows **all** work items under the selected epic — stories, tasks, bugs (including epic-direct leaves), not stories only.
3. When the user selects a **story** from that list, show the child list renamed from **Tasks** to **Sub Tasks** (tasks/bugs under that story).

## Acceptance criteria

- [ ] After selecting an epic in Overall, the middle list is labeled **Work items** (not Stories).
- [ ] Work items under an epic includes stories, epic-direct tasks/bugs, and any other non-epic children of the epic.
- [ ] Selecting a story opens the child list labeled **Sub Tasks** (not Tasks).
- [ ] Selecting a non-story work item does not open a Sub Tasks list (or behaves consistently with no children).
- [ ] Existing Overall filters, pagination, search, and detail-sheet open still work on these lists.

## Notes

Builds on S-025 / T-082 Overall drill-down; naming aligns with the Work items tab language.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:39:11Z | prompt | Marco Mendão | Remake Overall: Stories→Work items (all epic children); Tasks→Sub Tasks when story selected |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
