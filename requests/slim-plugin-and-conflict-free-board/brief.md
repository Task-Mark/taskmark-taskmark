---
id: R-slim-plugin-and-conflict-free-board
type: request
title: Slim plugin and conflict-free board
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-08-28
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - plugin
  - collaboration
  - board
  - commands
aliases:
  - E-022
source_meetings: []
links: []
---

# Slim plugin and conflict-free board

## Goal

Arrumar a casa: the Taskmark Cursor plugin exposes four commands, git stops fighting over generated board files, agents only touch leaf markdown, IDs do not collide, and unused plugin surface is deleted.

## Scope

- User commands: `/tsmk-init`, `/tsmk-create`, `/tsmk-commit`, `/tsmk-do` only. Delete every other slash command.
- `/tsmk-create` creates an epic, story, and/or task (including a full tree from a description).
- `/tsmk-do` implements work and never commits. It does not move items through `in_progress`. When the agent stops, executed leaves are `done`.
- `/tsmk-commit` is the only commit entrypoint.
- Remove `INDEX.md`, `SIZING.md`, `VELOCITY.md`, and board `README.md` (no changelog).
- Static sizing: XS=1, S=3, M=5, L=8, XL=13, XXL=21 with the agreed meanings.
- `REPOS.md` gitignored and generated locally (no absolute paths on the remote).
- No Last synced (or git-log changelog) in committed files.
- Create and do change only new/target leaf files — not parent `epic.md` / `story.md` lists or rollups. UI queries children.
- Parent Prompt & feedback, Commits, Work log, status, implementers, and lifecycle dates are read-time views over descendant leaves.
- Race-free IDs (not a global sequential T-NNN counter).
- Delete unused scripts, rules, hooks, commands, and skills.

## Done when

- Two people can create and finish different tasks without merging INDEX/README/SIZING/VELOCITY/parent files.
- Users see exactly four Taskmark slash commands.
- `/tsmk-do` never produces a git commit; leaves it worked are `done`.
- A new board has no INDEX, SIZING, VELOCITY, or README.

## Out of scope

- Changing product git commit style beyond `/tsmk-commit`.
- Rebuilding the marketing site except command/sizing docs.
- Migrating historical item IDs (old sequential IDs remain valid).
- Reintroducing velocity, README changelog, or start-work/complete-work as user commands.

## Open questions

_None yet._
