---
id: S-MO-4be0202b
type: story
title: File spec and structure match leaf-only boards
status: backlog
priority: high
size: L
points: 8
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [docs, specification]
created: 2026-08-28
updated: 2026-08-28T23:15:25Z
started_at: null
completed_at: null
---

# S-MO-4be0202b: File spec and structure match leaf-only boards

## User story

As someone reading or hand-editing board markdown, I want the file specification and folder-structure docs to match what `/tkmd-create` writes so I do not copy obsolete frontmatter, table headings, or a General epic.

## Acceptance criteria

- [ ] Frontmatter examples use current fields only (no estimate/owner; no `size_source` / `points_source` unless the parser still requires them).
- [ ] ID examples include `E|S|T|B-<identity>-<random>` and note that legacy `T-001`-style IDs remain valid.
- [ ] Epic and story templates have no child lists, rollups, Prompt & feedback, Commits, or Work log; those live on task/bug leaves.
- [ ] Leaf table headings and columns match conventions (`Prompt & feedback` without a `#` column; Work log Actor / Started / Ended / Summary).
- [ ] Structure docs cover single-repo `taskmark/` vs sibling `<common>-taskmark`, gitignored `REPOS.md`, and the absence of INDEX, SIZING, VELOCITY, and board README.
- [ ] The General epic section is removed or rewritten to match current create behaviour (create a parent when needed; do not imply a reserved General epic if it is no longer required).
