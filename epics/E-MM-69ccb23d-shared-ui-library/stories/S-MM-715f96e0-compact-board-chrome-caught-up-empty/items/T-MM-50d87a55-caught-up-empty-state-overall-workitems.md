---
id: T-MM-50d87a55
type: task
title: Show a caught-up empty state on Overall and Work items
status: done
priority: high
size: S
points: 3
parent: S-MM-715f96e0
epic: E-MM-69ccb23d
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
tags: [ui, board, empty-state]
created: 2026-09-15
updated: 2026-09-15T22:28:00Z
started_at: 2026-09-15T22:11:00Z
completed_at: 2026-09-15T22:28:00Z
---
# T-MM-50d87a55: Show a caught-up empty state on Overall and Work items

## Description

When Overall or Work items has board data but no remaining open work (typically hide-completed on and every leaf complete), show a distinct caught-up empty state instead of the filter-mismatch copy. Keep the existing empty board and active-search/filter messages.

## Acceptance criteria

- [x] Overall shows a caught-up empty state when the tree has items but none remain to do.
- [x] The Work items tab shows the same kind of empty state when the list has items but none remain to do.
- [x] An empty board still uses the existing no-items copy.
- [x] Search, parent, tag, or timeframe filters that hide remaining rows still use the filter-mismatch copy.
- [x] The empty state appears on local, npx static, and Cloud boards.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T22:11:00Z | prompt | Marco Mendão | Add a caught-up empty state on Overall and Work items when there are no remaining tasks to do, on local, npx, and Cloud boards. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T22:11:00Z | 2026-09-15T22:28:00Z | Added a caught-up empty state on Overall and Work items when hide-completed leaves no open work. |
