---
id: R-user-stories-view
type: request
title: User stories view
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
  - stories
  - frontend
aliases:
  - E-002
source_meetings: []
links: []
---

# User stories view

## Goal

Let users drill from an epic into its user stories, then from a selected story into the tasks connected to that story—so the dashboard shows the full epic → story → task hierarchy.

## Scope

- Select an epic (from the existing epic list or an epic picker) and show all user stories under that epic.
- Select a user story and show all tasks (and bugs) connected to that story.
- Parse story and item markdown from the local Taskmark board for the active project.
- Present id, title, status, size, points, and related summary fields for stories and tasks.
- Empty and error states when an epic has no stories or a story has no items.

## Done when

- From the dashboard, a user can pick an epic and see every story under it.
- Selecting a story reveals its connected tasks/bugs without leaving the drill-down flow.
- Parse failures for individual files do not break the whole view.

## Out of scope

- Editing board files from the UI.
- Creating or reordering stories/tasks in the UI.
- Full markdown body / work-log detail panes (beyond list summary fields).
- Cross-project story views (stories are scoped to the selected epic’s project board).

## Open questions

_None yet._
