---
id: S-039
type: story
title: Git identity data model
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 75
actual_minutes: 0
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-011
epic: E-011
owner: ""
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
tags: [identity, git, conventions, plugin]
created: 2026-07-23
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 0
---

# S-039: Git identity data model

## User story

As a Taskmark user, I want work items to store the people who reported and resolved them (name, email, initials from git config) so that attribution is durable and available to the UI and README.

## Acceptance criteria

- [x] Conventions document a contributor identity shape: `name`, `email`, and `initials` (derived when missing).
- [x] Epics, stories, tasks, and bugs can store `reporters` and `resolvers` (arrays; multi-author supported).
- [x] A shared helper can read `git config user.name` / `user.email` and produce initials.
- [x] Templates and frontmatter guidance cover the new fields.

## Tasks

- [T-111: Define contributor identity schema in conventions](items/T-111-contributor-identity-schema.md)
- [T-112: Add reporters and resolvers frontmatter on work items](items/T-112-reporters-resolvers-frontmatter.md)
- [T-113: Git config identity helper (name, email, initials)](items/T-113-git-config-identity-helper.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T17:28:57Z | prompt | Marco Mendão | Start developing E-011 (story scope). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:28:57Z | 2026-07-23T17:28:57Z | rollup: children hold shared-batch; delivered story |
