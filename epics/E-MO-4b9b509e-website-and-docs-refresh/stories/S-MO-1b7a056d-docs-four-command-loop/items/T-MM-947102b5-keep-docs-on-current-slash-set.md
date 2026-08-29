---
id: T-MM-947102b5
type: task
title: Keep docs on the current slash set
status: done
priority: high
size: XS
points: 1
parent: S-MO-1b7a056d
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [docs, commands]
created: 2026-08-29
updated: 2026-08-29T11:41:21Z
started_at: 2026-08-29T11:38:00Z
completed_at: 2026-08-29T11:38:20Z
---

# T-MM-947102b5: Keep docs on the current slash set

## Description

The parent story still describes a four-command loop (`/tkmd-create` and exactly four slashes). That model is obsolete. Public docs must keep the current set and must not be rewritten back to four commands only.

## Acceptance criteria

- [x] Overview, setup, commands, workflows, and docs nav name `/tkmd-init`, `/tkmd-plan`, `/tkmd-save`, `/tkmd-plan-do`, `/tkmd-do`, `/tkmd-shelf`, and `/tkmd-commit`.
- [x] Copy does not tell visitors to use only four slashes or `/tkmd-create`.
- [x] Searchable leftovers (`/tsmk`, `/new-epic`, `/create-task`, `/start-work`, `/commit-all`) stay absent from current docs copy.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:37:37Z | prompt | Marco Mendão | Review E-MO-4b9b509e stories; update or drop work that is already done. Four-command docs no longer match the product. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:38:00Z | 2026-08-29T11:38:20Z | Confirmed docs already list the current seven slashes; no four-command rewrite. |
