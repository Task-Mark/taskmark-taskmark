---
id: R-mvp-taskmark-dashboard
type: request
title: MVP Taskmark dashboard
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
  - mvp
  - dashboard
  - frontend
aliases:
  - E-001
source_meetings: []
links: []
---

# MVP Taskmark dashboard

## Goal

Ship an MVP dashboard that reads Taskmark markdown boards from a local **master folder** (a workspace that may contain multiple projects) and presents a clear view of the work. Near-term delivery focuses on a setup wizard to select that master folder, discovering Taskmark projects in its subfolders, and listing epics **per project**. Longer-term, the same board reader should power a complete epic / story / task dashboard.

## Scope

- Setup wizard: user selects a local **master folder** (workspace root), not necessarily a single repo with `taskmark/` at its root.
- Discover one or more Taskmark projects by scanning **subfolders** for `taskmark/` board files.
- Persist the selected **master folder** path in a **cookie** so returning users skip setup when already configured.
- Allow switching master folders by re-entering setup; cookie overwritten on switch.
- Validate that the master folder yields at least one discoverable Taskmark project (or guide the user clearly when none are found).
- Read and parse epic markdown under each discovered project’s `taskmark/epics/`.
- Show a list of epics **for each** discovered project (id, title, status, size, points, and related summary fields).

## Done when

- A user can open the app, pick a master folder that contains multiple Taskmark projects in subfolders, and see epics grouped (or listed) per project.
- Master folders with no discoverable boards are handled with clear feedback.
- Selected master folder path is remembered in a cookie across sessions; setup is not required again until the user switches or the cookie is gone.

## Out of scope

- Full story / task / bug detail views and nested drill-down (beyond what is needed to list epics).
- Editing board files from the UI.
- Favorites / parallel unrelated workspaces beyond one master-folder cookie for MVP.
- Cloud sync, accounts, or remote boards.

## Open questions

_None yet._
