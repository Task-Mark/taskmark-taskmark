---
id: E-010
type: epic
title: List search and filters
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 30
points_source: rolled_up
estimate_minutes: 460
actual_minutes: 16
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [dashboard, frontend, lists, search, filters]
created: 2026-07-23
updated: 2026-07-28T09:08:49.505Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-27T05:18:44Z
actual_ms: 1004000
---
# E-010: List search and filters

## Goal

Let users find and narrow work items quickly: every list has a search box (by id/code or title), the Work items tab adds parent epic/story autocomplete and multiselect tag filters, and a hide-completed control can hide done epics, stories, and tasks/bugs.

## Scope

- Shared search box matching work-item id (code) and title text (case-insensitive).
- Search on Overall epic, story, and task lists, and on the Work items list.
- Work items: autocomplete dropdown to filter by parent epic and/or story.
- Multiselect filter by frontmatter tags.
- Toggle/filter to hide completed (done) epics, stories, and tasks/bugs.
- Filters compose with existing pagination (reset to page 1 when filters change).

## Out of scope

- Full-text search across markdown body sections (goal/description only via title/id for v1).
- Saved filter presets or URL-synced filter state (optional later).
- Server-side search indexes.

## Success metrics

- User can type an id or title fragment and see matching rows on every main list.
- On Work items, parent and tag filters further narrow results; hide-completed removes done rows across lists.
- Empty filter results show a clear empty state; clearing filters restores the full list.

## Stories

- [S-033: Shared search control](stories/S-033-shared-search-control/story.md)
- [S-034: Search on Overall drill-down lists](stories/S-034-search-overall-lists/story.md)
- [S-035: Search on Work items list](stories/S-035-work-items-search/story.md)
- [S-036: Parent epic/story autocomplete filter](stories/S-036-parent-autocomplete-filter/story.md)
- [S-037: Tags multiselect filter](stories/S-037-tags-multiselect-filter/story.md)
- [S-038: Hide completed filter](stories/S-038-hide-completed-filter/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 66b89f7 | taskmark-frontend | 2026-07-23T16:17:20Z | Marco Mendão | add list search and filters |
| c964895 | taskmark-taskmark | 2026-07-23T16:17:33Z | Marco Mendão | complete e-010 list search and filters |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered E-010 list search and filters |
| 2 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:17:33Z | auto-recovered: commit span |
