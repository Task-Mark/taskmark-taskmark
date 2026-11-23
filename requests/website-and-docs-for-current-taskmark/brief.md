---
id: R-website-and-docs-for-current-taskmark
type: request
title: Website and docs for current Taskmark
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MO
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MO
created: 2026-08-28
updated: 2026-08-28T23:15:25Z
forecast: null
tags:
  - website
  - docs
  - marketing
aliases:
  - E-MO-4b9b509e
source_meetings: []
links: []
---

# Website and docs for current Taskmark

## Goal

Bring the public website, product docs, and repo READMEs in line with the slim plugin: four `/tkmd-*` commands, collision-resistant IDs, leaf-only markdown, static sizing, no generated board files, and the hierarchical Overall list.

## Scope

- Landing page copy, features, console demo, and board visual
- Docs under `taskmark-website` (setup, commands, structure, specification, sizing, workflows, overview)
- Board UI behaviour that users need to understand (Overall tree, derived parent views)
- Cursor plugin and linked-repo READMEs, plus marketplace description if it is user-facing
- Remove or redirect leftover velocity, README-dashboard, changelog, sequential-ID-only, and General-epic guidance

## Done when

- A visitor can install, init, create, do, and commit using only `/tkmd-init`, `/tkmd-create`, `/tkmd-do`, and `/tkmd-commit`
- File specification matches what `/tkmd-create` writes today (IDs, frontmatter, leaf tables)
- No public page still teaches INDEX/SIZING/VELOCITY/board README, `in_progress`, or velocity ETA as current product
- Overall is described as a nested hierarchy, not three stacked tables

## Out of scope

- Implementing product commands or board UI (those live in other epics)
- Translating the site
- Changing commit or publish automation beyond documenting `/tkmd-commit`

## Open questions

_None yet._
