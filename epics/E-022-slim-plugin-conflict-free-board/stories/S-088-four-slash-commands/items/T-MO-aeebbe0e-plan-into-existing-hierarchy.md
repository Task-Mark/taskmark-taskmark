---
id: T-MO-aeebbe0e
type: task
title: Fit planned work into the existing hierarchy
status: backlog
priority: high
size: L
points: 8
parent: S-088
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, planning, hierarchy, deduplication]
created: 2026-08-29
updated: 2026-08-29T10:39:07Z
started_at: null
completed_at: null
---

# T-MO-aeebbe0e: Fit planned work into the existing hierarchy

## Description

Before creating files, `/tkmd-plan` must inspect the canonical board and place
new work under the best existing epic or story when the scope fits. It may
create missing parents or a new hierarchy only when no existing item provides
the right product context.

## Acceptance criteria

- [ ] The skill searches open and done board items for matching scope before allocating IDs.
- [ ] New tasks/bugs can be attached to an existing story or directly to an existing epic using frontmatter relationships.
- [ ] A new story can be attached to an existing epic without editing that epic file.
- [ ] A new epic is created only for a distinct initiative/outcome that does not fit an existing epic.
- [ ] Creation remains conflict-resistant: only new item files are written, existing parents and leaves are never rewritten.
- [ ] The resulting hierarchy avoids duplicate work items and preserves leaf-only prompt/feedback conventions.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:38:00Z | prompt | Marco Mendão | Rename `/tkmd-create` to `/tkmd-plan` and make it organize user requirements into the optimal Taskmark hierarchy. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
