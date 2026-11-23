---
id: R-list-search-and-filters
type: request
title: List search and filters
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-23
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - dashboard
  - frontend
  - lists
  - search
  - filters
aliases:
  - E-010
source_meetings: []
links: []
---

# List search and filters

## Goal

Let users find and narrow work items quickly: every list has a search box (by id/code or title), the Work items tab adds parent epic/story autocomplete and multiselect tag filters, and a hide-completed control can hide done epics, stories, and tasks/bugs.

## Scope

- Shared search box matching work-item id (code) and title text (case-insensitive).
- Search on Overall epic, story, and task lists, and on the Work items list.
- Work items: autocomplete dropdown to filter by parent epic and/or story.
- Multiselect filter by frontmatter tags.
- Toggle/filter to hide completed (done) epics, stories, and tasks/bugs.
- Filters compose with existing pagination (reset to page 1 when filters change).

## Done when

- User can type an id or title fragment and see matching rows on every main list.
- On Work items, parent and tag filters further narrow results; hide-completed removes done rows across lists.
- Empty filter results show a clear empty state; clearing filters restores the full list.

## Out of scope

- Full-text search across markdown body sections (goal/description only via title/id for v1).
- Saved filter presets or URL-synced filter state (optional later).
- Server-side search indexes.

## Open questions

_None yet._
