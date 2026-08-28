---
id: T-272
type: task
title: Strip work-item IDs from changelog entry text
status: backlog
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 20
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:11min/pt]
session_cap_minutes: 480
parent: S-087
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
updated: 2026-08-28T12:37:43.783Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-272: Strip work-item IDs from changelog entry text

## Description

Ensure generators/filters remove or rewrite ID-prefixed titles before writing README bullets.

## Acceptance criteria

- [ ] No T-/B-/S-/E- codes appear in Development or released changelog bullets.
- [ ] Existing ID-heavy commit subjects are transformed or replaced.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T07:21:00Z | prompt | Marco Mendão | Create epic for new version generator with stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
