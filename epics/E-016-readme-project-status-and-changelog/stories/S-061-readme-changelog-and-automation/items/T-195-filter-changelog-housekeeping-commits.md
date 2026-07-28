---
id: T-195
type: task
title: Filter housekeeping commits from README changelog
status: done
priority: medium
size: M
size_source: suggested
size_basis: [calibrated:T-195]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-195]
session_cap_minutes: 480
parent: S-061
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
tags: [readme, changelog, plugin]
created: 2026-07-27
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-27T07:39:00Z
completed_at: 2026-07-27T07:42:24Z
actual_ms: 204000
---
# T-195: Filter housekeeping commits from README changelog

## Description

README changelog should list meaningful board/product changes only — exclude routine sync/housekeeping commits such as `sync taskmark board` and `update readme dashboard`.

## Acceptance criteria

- [x] `refresh-readme-dashboard.py` omits known housekeeping subjects from the Changelog table
- [x] Overscan git log so the visible row limit still fills after filtering
- [x] Docs describe which commit messages are excluded
- [x] Regenerated board README changelog has no `sync taskmark board` rows

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T07:40:00Z | prompt | Marco Mendão | Dont show the sync taskmark board on the changelog only meaningfull changing commits and changes. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 0c7bfa3 | taskmark-cursor | 2026-07-27T07:46:37Z | Marco Mendão | filter changelog housekeeping commits |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T07:39:00Z | 2026-07-27T07:42:24Z | Filter housekeeping subjects from README changelog; overscan git log; docs |
