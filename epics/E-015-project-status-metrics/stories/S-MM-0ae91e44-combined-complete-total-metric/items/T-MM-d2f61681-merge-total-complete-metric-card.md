---
id: T-MM-d2f61681
type: task
title: Merge Total and Complete into one fraction card
status: done
priority: medium
size: S
points: 3
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
tags: [frontend, metrics]
created: 2026-08-30
updated: 2026-08-30T07:06:06Z
started_at: 2026-08-30T06:57:15Z
completed_at: 2026-08-30T07:06:06Z
---

# T-MM-d2f61681: Merge Total and Complete into one fraction card

Replace the two Overall metric cards (Total work items and Complete work items) with a single card titled Complete work items. The large value is `total/complete` (for example `500/400`). Keep the existing neo-brutalism card chrome. Do not change Current week, speed, contributors, or the heatmap.

## Acceptance criteria

- [x] Only one work-item count card remains on live and static Overall.
- [x] Title is Complete work items; value is `total/complete` with tabular numerals.
- [x] Subtitle still makes clear the count is stories, bugs, and tasks (epics excluded).
- [x] Layout still reads well in the metrics row on desktop and mobile after dropping a card.

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
| Marco Mendão | 2026-08-30T06:57:15Z | 2026-08-30T07:06:06Z | Merged Total and Complete into one fraction card |
