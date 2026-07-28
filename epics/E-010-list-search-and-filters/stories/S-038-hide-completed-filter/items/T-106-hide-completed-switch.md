---
id: T-106
type: task
title: Hide completed control as switch
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-103]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-038
epic: E-010
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
tags: [dashboard, frontend, filters]
created: 2026-07-23
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-23T16:14:35Z
completed_at: 2026-07-23T16:16:45Z
actual_ms: 130000
---

# T-106: Hide completed control as switch

## Description

Replace the Hide completed checkbox with the shared Switch UI control.

## Acceptance criteria

- [x] Hide completed uses a switch (not a native checkbox).
- [x] Default remains off; behavior unchanged.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:14:35Z | prompt | Marco Mendão | hide complete should be a switch |
| 2 | 2026-07-23T16:16:45Z | feedback | Marco Mendão | switch control wired |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:14:35Z | 2026-07-23T16:16:45Z | Delivered Hide completed as Switch |
