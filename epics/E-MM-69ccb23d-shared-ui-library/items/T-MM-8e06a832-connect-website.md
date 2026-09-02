---
id: T-MM-8e06a832
type: task
title: Connect website to shared components
status: done
priority: medium
size: M
points: 5
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
tags: [website, ui]
created: 2026-09-02
updated: 2026-09-02T08:14:16Z
started_at: 2026-09-02T07:51:50Z
completed_at: 2026-09-02T08:14:16Z
---
# T-MM-8e06a832: Connect website to shared components

## Description

Replace duplicated website primitives, theme helpers, and brand components with imports from `@taskmark/components`.

## Acceptance criteria

- [x] Marketing and documentation components consume shared primitives.
- [x] Landing and site-specific composition remains in the website.
- [x] Website lint and build pass.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T07:51:50Z | prompt | Marco Mendão | Include the Taskmark website as a consumer of the common UI library. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T07:51:50Z | 2026-09-02T08:14:16Z | Removed duplicated website UI sources and connected shared exports. |
