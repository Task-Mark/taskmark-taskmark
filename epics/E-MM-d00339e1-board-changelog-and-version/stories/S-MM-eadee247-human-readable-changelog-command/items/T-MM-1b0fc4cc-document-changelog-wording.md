---
id: T-MM-1b0fc4cc
type: task
title: Document changelog wording without work-item IDs
status: done
priority: high
size: S
points: 3
parent: S-MM-eadee247
epic: E-MM-d00339e1
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
tags: [changelog, conventions]
created: 2026-08-29
updated: 2026-08-29T17:18:08Z
started_at: 2026-08-29T17:13:00Z
completed_at: 2026-08-29T17:18:08Z
---

# T-MM-1b0fc4cc: Document changelog wording without work-item IDs

## Description

Document how agents write Unreleased bullets: one user-visible outcome, past tense, from user story / acceptance / title, never IDs or commit shorthand. Example: “Foi adicionado um botão para filtrar as tarefas já realizadas.”

## Acceptance criteria

- [x] `taskmark-conventions` (and the changelog skill) state the wording rules and Portuguese Keep a Changelog headings (`Não publicado`, `## x.y.z - date`)
- [x] Merging related leaves from the same story is allowed when it reads better
- [x] Visible changelog text must not include work-item codes

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T16:56:10Z | prompt | Marco Mendão | `/tkmd-save`: Cursor plan for `/tkmd-changelog` and `/tkmd-version` with CHANGELOG.md on the board and version on taskmark-taskmark package.json. |
| 2026-08-29T17:13:00Z | prompt | Marco Mendão | `/tkmd-do`: implement every open descendant of epic E-MM-d00339e1. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T17:13:00Z | 2026-08-29T17:13:44Z | Documented Portuguese changelog wording without work-item IDs. |
