---
id: S-060
type: story
title: README open work items list
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 4
points_source: rolled_up
estimate_minutes: 0
actual_minutes: 0
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
updated: 2026-07-28T15:03:07.151Z
started_at: 2026-07-27T07:32:04Z
completed_at: 2026-07-27T07:36:40Z
actual_ms: 2000
---

# S-060: README open work items list

## User story

As a repo visitor, I want regenerate an open-only stories/tasks/bugs table in readme for repo visitors. so the board README stays useful without opening the UI.

## Acceptance criteria

- [x] Regenerate an open-only stories/tasks/bugs table in README for repo visitors.

## Tasks

- [T-190: Collect open work item rows](items/T-190-collect-open-work-rows.md)
- [T-191: Upsert README open work marker section](items/T-191-upsert-readme-open-work-section.md)

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
