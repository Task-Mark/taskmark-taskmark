---
id: E-MO-a3da5abd
type: epic
title: Hierarchical Overall task list
status: backlog
priority: high
size: null
points: null
parent: null
epic: null
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, overall, ux]
created: 2026-08-29
updated: 2026-08-28T23:03:00Z
started_at: null
completed_at: null
---

# E-MO-a3da5abd: Hierarchical Overall task list

## Goal

Replace Overall’s stacked epic, work-item, and sub-task tables with one nested list so people scan the board as a hierarchy: epics first, then stories and epic-direct work under an opened epic, then tasks and bugs under an opened story.

## Scope

- Overall is a single hierarchical surface (tree table or equivalent), not three separate tables.
- Expanding an epic reveals its stories and epic-direct tasks/bugs beneath it.
- Expanding a story reveals its tasks and bugs beneath that story.
- Default order at every level: incomplete before complete, then newest first.
- Strong expand/collapse UX: clear affordances, indent, type/status chrome, open detail without losing expand state.
- Search, hide-completed, timeframe, pagination, static board, and deep links still work on this tree.
- All, Stories, and Tasks views stay as they are.

## Out of scope

- Creating or editing items from Overall.
- Changing markdown hierarchy or frontmatter.
- Redesigning All / Stories / Tasks tables.
- Multi-project aggregation beyond the active board.

## Success metrics

- Overall no longer uses stacked independent tables for epics, work items, and sub-tasks.
- A user can reach any task by expanding its epic and story in place.
- Incomplete work surfaces above completed work; newer items surface above older ones at each level.
- Filters and the work-item sheet still work without collapsing the hierarchy unexpectedly.
