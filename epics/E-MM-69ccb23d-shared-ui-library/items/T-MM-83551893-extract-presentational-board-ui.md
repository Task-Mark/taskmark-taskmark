---
id: T-MM-83551893
type: task
title: Extract presentational board UI
status: done
priority: high
size: L
points: 8
parent: E-MM-69ccb23d
epic: E-MM-69ccb23d
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
tags: [ui, board]
created: 2026-09-02
updated: 2026-09-02T09:11:44Z
started_at: 2026-09-02T07:51:50Z
completed_at: 2026-09-02T08:14:16Z
---
# T-MM-83551893: Extract presentational board UI

## Description

Expose reusable board chrome and presentational work-item components through view models and callback-driven APIs.

## Acceptance criteria

- [x] The package exports a reusable Taskmark app bar and board shell.
- [x] Shared board components do not import frontend server actions or filesystem loaders.
- [x] Cloud can render a Taskmark-style board surface from supplied data.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T07:51:50Z | prompt | Marco Mendão | Make the local and cloud Taskmark interfaces reusable without duplicating board UI. |
| 2026-09-02T09:11:44Z | feedback | Marco Mendão | The shared top bar had been rebuilt instead of reused, dropping the hover underline, the product tagline, and the no-script project switching. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T07:51:50Z | 2026-09-02T08:14:16Z | Added callback-driven app chrome and a data-driven board surface. |
| Marco Mendão | 2026-09-02T09:06:23Z | 2026-09-02T09:11:44Z | Rebuilt the shared top bar as an exact port of the original chrome, with each product supplying its own controls. |
