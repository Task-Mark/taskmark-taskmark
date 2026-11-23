---
id: R-optional-hierarchy-and-general-epic
type: request
title: Optional hierarchy and General epic
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
  - plugin
  - conventions
  - hierarchy
  - dashboard
aliases:
  - E-007
source_meetings: []
links: []
---

# Optional hierarchy and General epic

## Goal

Let stories and tasks exist without a required parent, while still preferring a contextual epic/story when one is clear, and house general tasks and user stories under a default **General** epic visible in the epic list.

## Scope

- Optional `parent` / `epic` for stories and tasks (null allowed).
- Create skills infer parents from prompt/context when the user does not name one.
- Fallback attachment to a board-default **General** epic (and a catch-all story under it when a task has no story).
- Dashboard epic list always includes General so general tasks and user stories are discoverable.
- Conventions, init, create skills, and UI/parser updates needed for the above.

## Done when

- Creating a story or task without an explicit parent succeeds.
- General tasks and user stories appear under General in the epic list (epic `items/` + stories; no Unattached story).
- Explicit or clearly contextual parents still win over General.

## Out of scope

- Deleting or flattening existing epic → story → task trees.
- Free-form items outside the board markdown model.
- Renaming or merging user epics into General automatically.

## Open questions

_None yet._
