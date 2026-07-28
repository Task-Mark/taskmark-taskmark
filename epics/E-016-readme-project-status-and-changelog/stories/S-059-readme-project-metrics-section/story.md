---
id: S-059
type: story
title: README project metrics section
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 4
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
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-27T07:32:04Z
completed_at: 2026-07-27T07:36:40Z
actual_ms: 120000
---

# S-059: README project metrics section

## User story

As a repo visitor, I want add a managed readme section with total, complete, and current speed matching e-015. so the board README stays useful without opening the UI.

## Acceptance criteria

- [x] Add a managed README section with Total, Complete, and Current Speed matching E-015.

## Tasks

- [T-188: Compute README metrics from board leaves](items/T-188-compute-readme-metrics.md)
- [T-189: Upsert README metrics marker section](items/T-189-upsert-readme-metrics-section.md)

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
