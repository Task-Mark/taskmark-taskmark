---
id: R-view-work-item
type: request
title: View work item
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-21
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - dashboard
  - frontend
  - detail
  - sheet
aliases:
  - E-005
source_meetings: []
links: []
---

# View work item

## Goal

Let users open any work item (epic, user story, or task) in a dedicated view mode that presents every available detail in the clearest layout, always inside a sheet.

## Scope

- View mode for epics, user stories, and tasks (bugs use the same item view as tasks where applicable).
- Present all work-item information in the best layout for each type (frontmatter fields, goal/user story/description, acceptance criteria, children, work log, commits, prompt & feedback, timing, and related metadata).
- Every work-item view is presented in a sheet (slide-over / drawer), not a full-page route replacement.
- Open the sheet from existing list UIs (epic, story, and task lists) without breaking the current drill-down hierarchy.
- Empty and error states when a selected item cannot be loaded or has sparse content.

## Done when

- From any epic, story, or task list row, the user can open that item’s detail view in a sheet.
- The sheet shows the item’s details clearly and appropriately for its type.
- Closing the sheet returns the user to the same list/drill-down context.

## Out of scope

- Editing or creating work items from the sheet.
- Separate full-page detail routes.
- Cross-project detail views (scoped to the active project board).
- Reordering or bulk actions from the sheet.

## Open questions

_None yet._
