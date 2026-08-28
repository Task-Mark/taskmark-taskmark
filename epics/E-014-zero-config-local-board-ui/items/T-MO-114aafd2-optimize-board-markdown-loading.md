---
id: T-MO-114aafd2
type: task
title: Optimize board markdown loading
status: done
priority: high
size: L
points: 8
parent: E-014
epic: E-014
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
tags: [frontend, performance, markdown, rollup]
created: 2026-08-28
updated: 2026-08-28T16:08:45Z
started_at: 2026-08-28T16:02:21Z
completed_at: 2026-08-28T16:08:45Z
---

# T-MO-114aafd2: Optimize board markdown loading

## Description

Build one in-memory board index per request so parent rollups, lists, and metrics
reuse parsed markdown instead of repeatedly scanning every board file.

## Acceptance criteria

- [x] Task and bug frontmatter is read once for normal list and metrics rendering.
- [x] Parent rollups use leaves grouped by epic and story.
- [x] Detail tables are parsed only when parent detail aggregation needs them.
- [x] BoardScreen reuses one board index and does not collect metrics twice.
- [x] Relevant tests, lint, and build pass.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-28T16:08:45Z | prompt | Marco Mendão | Implement the suggested single-scan markdown loading optimizations. |
| 2026-08-28T22:36:27Z | prompt | Marco Mendão | Group duplicate prompt/work-log rows; show work items as aligned tags. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-28T16:02:21Z | 2026-08-28T16:08:45Z | Added a reusable board index, lazy detail parsing, and shared metric collection; verified sub-second application rendering. |
