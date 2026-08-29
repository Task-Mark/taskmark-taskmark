---
id: T-265
type: task
title: Suggest semver bump from changes since last release
status: shelved
priority: high
size: L
size_source: suggested
size_basis: []
points: 5
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:10min/pt]
session_cap_minutes: 480
parent: S-085
epic: E-021
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [release, versioning, changelog, readme, plugin]
created: 2026-07-29
updated: 2026-08-29T11:09:34Z
started_at: null
completed_at: 2026-08-29T11:09:34Z
actual_ms: 0
---
# T-265: Suggest semver bump from changes since last release

## Description

Analyze commits/board work since the last released version and recommend major/minor/patch.

## Acceptance criteria

- [ ] Produces a suggested version when the user does not supply one.
- [ ] Suggestion is grounded in change scope (breaking / feature / fix), not calendar time.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T07:21:00Z | prompt | Marco Mendão | Create epic for new version generator with stories and tasks |
| 2 | 2026-08-29T11:09:34Z | prompt | Marco Mendão | Shelve incomplete work on E-001, E-014, and E-021 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
