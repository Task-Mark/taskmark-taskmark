---
id: T-122
type: task
title: Multi-avatar stack and same-person dedupe
status: done
priority: high
size: S
size_source: suggested
size_basis: [velocity:similar]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-042
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
tags: [frontend, avatars, ux]
created: 2026-07-23
updated: 2026-07-28T06:16:13.686Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---
# T-122: Multi-avatar stack and same-person dedupe

## Description

When building the avatar group for a row: merge reporters and resolvers by email; if one person both created and resolved, show a single avatar with “Created and developed by &lt;name&gt;”; otherwise show separate avatars with “Created by …” / “Resolved by …”; support multiple people.

## Acceptance criteria

- [x] Same email across reporter+resolver → one avatar + combined hover text.
- [x] Distinct people → multiple avatars with role-appropriate hover text.
- [x] Multiple reporters or resolvers all appear (stacked/grouped).

## Notes

Hover copy should use proper phrasing: “Created by”, “Resolved by”, “Created and developed by”.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T17:28:57Z | prompt | Marco Mendão | User asked to start developing epic E-011. |
| 2 | 2026-07-23T17:36:57Z | feedback | Marco Mendão | Delivered identity schema, git helper, README sync, list avatars, activity authors. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:32:57Z | 2026-07-23T17:33:57Z | delivered; shared-batch: 1 of 8min by points |
