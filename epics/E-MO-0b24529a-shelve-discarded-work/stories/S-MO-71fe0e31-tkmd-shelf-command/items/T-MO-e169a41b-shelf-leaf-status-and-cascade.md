---
id: T-MO-e169a41b
type: task
title: Shelf leaf status and cascade descendants
status: done
priority: high
size: M
points: 5
parent: S-MO-71fe0e31
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
tags: [plugin, conventions]
created: 2026-08-29
updated: 2026-08-29T11:06:17Z
started_at: 2026-08-29T10:58:00Z
completed_at: 2026-08-29T11:03:58Z
---

# T-MO-e169a41b: Shelf leaf status and cascade descendants

## Description

Define `status: shelved` as discarded, never-implemented, terminal work. `/tkmd-shelf` writes only descendant task/bug leaves (or the targeted leaf). `/tkmd-do` skips already-shelved leaves the way it skips cancelled ones.

## Acceptance criteria

- [x] Conventions document `shelved` as a complete/discarded leaf status, distinct from `done`.
- [x] Shelving a leaf sets `status: shelved` and `completed_at`; does not set `cancelled: true`; does not rewrite parent markdown.
- [x] Shelving a story or epic applies that write to every open, non-cancelled, non-shelved descendant leaf.
- [x] `/tkmd-do` does not require shelved descendants to become `done`.

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
| Marco Mendão | 2026-08-29T10:58:00Z | 2026-08-29T10:59:52Z | Defined shelved leaf semantics, parent cascade, and tkmd-do exclusion. |
| Marco Mendão | 2026-08-29T11:05:00Z | 2026-08-29T11:05:24Z | Covered shelved semantics and tkmd-do exclusions in plugin contract tests. |
