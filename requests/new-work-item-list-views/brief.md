---
id: R-new-work-item-list-views
type: request
title: New work item list views
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-22
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - dashboard
  - frontend
  - views
  - lists
aliases:
  - E-006
source_meetings: []
links: []
---

# New work item list views

## Goal

Let users switch the board between Overall (current drill-down), All (flat mixed table), Stories (stories with epic tags), and Tasks (tasks with epic and story tags) via a button-group control.

## Scope

- A view switcher control (button group / segmented control) for Overall, All, Stories, and Tasks.
- Overall: preserve the current epic → story → task nested view as the default.
- All: one table with every epic, story, and task/bug.
- Stories: stories only, each with a UI tag for its parent epic.
- Tasks: tasks/bugs only, each with UI tags for parent epic and story.
- Open existing work item detail sheets from the new list rows.

## Done when

- User can switch among the four views with one control.
- Overall remains the default and matches today’s drill-down.
- All / Stories / Tasks show the correct row sets with the specified parent tags.
- Detail sheets still open from list rows in every view.

## Out of scope

- Editing or creating items from the new views.
- Filtering, sorting, or saved custom views beyond the four modes.
- Changing Taskmark markdown frontmatter `tags` fields (view tags are UI parent badges).
- Cross-project aggregation beyond the active board.

## Open questions

_None yet._
