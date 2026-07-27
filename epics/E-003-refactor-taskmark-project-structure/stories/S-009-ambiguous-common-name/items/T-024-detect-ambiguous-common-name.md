---
id: T-024
type: task
title: Detect ambiguous common-name cases
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-020, T-008]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_basis: [calibrated:T-024]
session_cap_minutes: 480
parent: S-009
epic: E-003
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
tags: [multi-repo, naming, detection]
created: 2026-07-21
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-21T22:04:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 0
---

# T-024: Detect ambiguous common-name cases

## Description

Define when automatic common-name derivation is not confident enough (unrelated names, multiple plausible prefixes, conflicting parent folders) and surface an “ambiguous” result for prompting.

## Acceptance criteria

- [x] Explicit ambiguity conditions documented and implemented in the naming helper.
- [x] Ambiguous result blocks automatic folder creation until the user answers.
- [x] Clear cases still return a derived name without prompting.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for Taskmark project structure refactor |
| 2 | 2026-07-21T22:36:37Z | feedback | Marco Mendão | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:04:51Z | 2026-07-21T22:04:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0 of 1min by points |
