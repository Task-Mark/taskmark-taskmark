---
id: S-041
type: story
title: README contributors
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 80
actual_minutes: 1
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
tags: [identity, contributors, readme, plugin]
created: 2026-07-23
updated: 2026-07-24T16:57:53.518Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---
# S-041: README contributors

## User story

As a project maintainer, I want everyone who creates or resolves work items (via git identity) listed as contributors in the project README so the repo credits stay current.

## Acceptance criteria

- [x] Project README(s) have a Contributors section listing name (and email when available).
- [x] New identities discovered on create/resolve are upserted into that section (no duplicate emails).
- [x] Existing contributor entries are preserved; only missing people are added (or a managed generated block is refreshed safely).

## Tasks

- [T-117: Upsert Contributors section in project README](items/T-117-upsert-readme-contributors.md)
- [T-118: Sync README when a new git identity appears](items/T-118-sync-readme-on-new-identity.md)

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
