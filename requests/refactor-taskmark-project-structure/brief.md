---
id: R-refactor-taskmark-project-structure
type: request
title: Refactor Taskmark project structure
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
  - architecture
  - multi-repo
  - plugin
  - board-layout
aliases:
  - E-003
source_meetings: []
links: []
---

# Refactor Taskmark project structure

## Goal

Stop copying `taskmark/` into every product repo. Place the board where git ownership is clear: inside the sole project for single-repo workspaces, or in a dedicated sibling `<common_project_name>-taskmark` git project whose **root is the board** for multi-repo workspaces.

## Scope

- Single-folder / single-git workspaces: `taskmark/` lives inside that project and uses the project’s git history.
- Multi-folder / multi-git workspaces: create a sibling project named `<common_project_name>-taskmark` (ask the user when the common name is ambiguous).
- Initialize a new git repository for the dedicated multi-project Taskmark folder.
- Update plugin conventions, skills, scripts, and the always-apply rule to match the new model.
- Provide a migration path away from per-repo board copies.

## Done when

- Single-repo workspaces never create a sibling Taskmark project; board commits land in the product repo.
- Multi-repo workspaces have exactly one canonical board at `<name>-taskmark/` **root** (no nested `taskmark/`) with its own `.git`.
- Agents no longer sync/copy `taskmark/` into every linked product repo.
- Ambiguous naming always prompts the user before creating the dedicated project.

## Out of scope

- Changing epic/story/task markdown schema or INDEX format beyond repo-layout docs.
- Frontend dashboard UI redesign (discovery may need follow-up once layout lands).
- Hosting or remotes for the new Taskmark git repo (local `git init` only unless later requested).

## Open questions

_None yet._
