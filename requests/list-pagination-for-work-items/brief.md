---
id: R-list-pagination-for-work-items
type: request
title: List pagination for work items
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
  - pagination
aliases:
  - E-009
source_meetings: []
links: []
---

# List pagination for work items

## Goal

Every work-item list in the system (Overall epic/story/task tables and the Work items list) supports pagination with first / previous / next / last navigation and a page-size dropdown so large boards stay usable.

## Scope

- Shared pagination control: first, previous, next, last; current page indicator; page-size select.
- Apply pagination to Overall epic, story, and task lists.
- Apply pagination to the Work items tab list.
- Sensible default page sizes and disabled nav when at bounds.

## Done when

- User can change page size and move between pages on every main list.
- Nav controls disable correctly on first/last page.
- Empty and short lists still render cleanly (no broken controls).

## Out of scope

- Server-side / filesystem streaming pagination (client-side slice of already-loaded rows is enough).
- Infinite scroll.
- Persisting page index across navigation (page size persistence optional later).
- Paginating detail-sheet children lists.

## Open questions

_None yet._
