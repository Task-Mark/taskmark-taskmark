---
id: S-061
type: story
title: README changelog and automation
status: done
priority: medium
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 8
points_source: rolled_up
estimate_minutes: 0
actual_minutes: 2
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-016
epic: E-016
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
tags: [readme, metrics, changelog, plugin]
created: 2026-07-27
updated: 2026-07-27T07:37:31Z
started_at: 2026-07-27T07:32:04Z
completed_at: 2026-07-27T07:36:40Z
actual_ms: 121000
---

# S-061: README changelog and automation

## User story

As a repo visitor, I want add changelog section from board-repo commits and refresh readme on sync/complete/commit. so the board README stays useful without opening the UI.

## Acceptance criteria

- [x] Add changelog section from board-repo commits and refresh README on sync/complete/commit.

## Tasks

- [T-192: Upsert README changelog from board commits](items/T-192-upsert-readme-changelog.md)
- [T-193: Wire README refresh into sync and complete](items/T-193-wire-readme-refresh-into-sync.md)
- [T-194: Document README dashboard conventions](items/T-194-document-readme-dashboard.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T07:32:04Z | prompt | Marco Mendão | Implement this E-016 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 764379b | taskmark-cursor | 2026-07-27T07:37:20Z | Marco Mendão | add readme dashboard refresh |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T07:36:40Z | 2026-07-27T07:36:40Z | Parent rollup: children hold shared-batch |
