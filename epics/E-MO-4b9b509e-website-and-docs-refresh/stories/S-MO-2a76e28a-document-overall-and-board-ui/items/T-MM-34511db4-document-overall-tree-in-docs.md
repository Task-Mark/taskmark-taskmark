---
id: T-MM-34511db4
type: task
title: Document Overall tree in public docs
status: done
priority: high
size: M
points: 5
parent: S-MO-2a76e28a
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
tags: [docs, website, overall]
created: 2026-08-29
updated: 2026-08-29T11:41:21Z
started_at: 2026-08-29T11:39:55Z
completed_at: 2026-08-29T11:40:40Z
---

# T-MM-34511db4: Document Overall tree in public docs

## Description

Public docs still omit the hierarchical Overall list. Visitors need to know Overall is one nested tree, that other Work items views stay flat, and that parent status, points, people, dates, and logs are read-time views.

## Acceptance criteria

- [x] Docs explain Overall as a hierarchical tree: expand epic → stories and epic-direct work; expand story → tasks/bugs; incomplete then newest at each level.
- [x] Docs note that All, Stories, and Tasks views stay flat lists, and that search, hide-completed, timeframe, pagination, and deep links apply to the tree.
- [x] Docs explain derived parent views (status, points, Actual, implementers, lifecycle dates, aggregated logs) vs leaf-only writes.
- [x] How to open the local board (`@taskmark/ui`, bound vs workspace) is accurate relative to the frontend README.
- [x] Landing or docs do not show Overall as three stacked independent tables.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:37:37Z | prompt | Marco Mendão | Review E-MO-4b9b509e; Overall tree docs are still missing from the website. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:39:55Z | 2026-08-29T11:40:40Z | Documented Overall tree, Work items flat view, and how to open @taskmark/ui. |
