---
id: T-085
type: task
title: Date tooltips on ID and done badge instead of columns
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [calibrated:T-085]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 16
estimate_source: suggested
estimate_basis: [calibrated:T-085]
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
tags: [dashboard, frontend, views, workitems, dates, tooltip]
created: 2026-07-23
updated: 2026-07-27T05:37:38.663Z
started_at: 2026-07-23T07:51:22Z
completed_at: 2026-07-23T07:54:27Z
actual_ms: 971000
---
# T-085: Date tooltips on ID and done badge instead of columns

## Description

Remove Created/Solved columns from the Work items list. Show creation date as a tooltip on the item ID (code), and solved date as a tooltip on the done status badge. Apply the same pattern on Overall epic, story, and task lists.

## Acceptance criteria

- [x] Work items list has no Created or Solved columns.
- [x] Hovering the item ID shows the creation date.
- [x] Hovering a done status badge shows the solved date (`completed_at`).
- [x] Epic, story, and task Overall lists use the same ID and done-badge tooltips.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T07:51:22Z | prompt | Marco Mendão | Remove date columns; tooltip on ID for created, on done badge for solved |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 83d2ae9 | taskmark-frontend | 2026-07-23T08:04:28Z | Marco Mendão | add created solved date tooltips |
| 1cee199 | taskmark-taskmark | 2026-07-23T08:04:28Z | Marco Mendão | add t-084 t-085 date tooltip board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T07:51:22Z | 2026-07-23T07:54:27Z | Date tooltips on ID + done badge; removed columns |
| 2 | Marco Mendão | 2026-07-23T07:51:22Z | 2026-07-23T08:04:28Z | auto-recovered: commit span |
