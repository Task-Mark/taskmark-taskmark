---
id: T-MO-b0dbcafe
type: task
title: Document /tkmd-shelf and shelved status
status: done
priority: medium
size: S
points: 3
parent: S-MO-70254dfe
epic: E-MO-0b24529a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
blocked: false
cancelled: false
tags: [docs, website]
created: 2026-08-29
updated: 2026-08-29T11:06:17Z
started_at: 2026-08-29T10:58:00Z
completed_at: 2026-08-29T11:03:58Z
---

# T-MO-b0dbcafe: Document /tkmd-shelf and shelved status

## Description

Update website docs (and plugin README if it still advertises four commands) so `/tkmd-shelf` and `status: shelved` are part of the current product: discarded, never implemented, distinct from done, hidden by hide-completed.

## Acceptance criteria

- [x] Commands/workflows pages describe `/tkmd-shelf`.
- [x] Specification documents `shelved` status, leaf writes, and parent rollup.
- [x] Copy that claimed exactly four `/tkmd-*` commands includes shelf.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:53:00Z | prompt | Marco Mendão | New `/tkmd-shelf` to discard never-implemented tasks/epics/stories; distinct from done; hide-completed hides shelved. |
| 2026-08-29T11:03:58Z | prompt | Marco Mendão | Implement E-MO-0b24529a and all open descendant leaves. |
| 2026-08-29T11:06:17Z | feedback | Marco Mendão | Apply necessary follow-up findings from the completed implementation audits. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T10:58:00Z | 2026-08-29T10:59:08Z | Documented the shelf command, terminal status, rollups, and filtering. |
| Marco Mendão | 2026-08-29T11:05:00Z | 2026-08-29T11:05:15Z | Updated overview, setup, command, and landing workflow copy. |
