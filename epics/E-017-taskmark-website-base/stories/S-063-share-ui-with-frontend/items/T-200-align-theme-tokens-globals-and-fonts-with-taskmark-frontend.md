---
id: T-200
type: task
title: Align theme tokens globals and fonts with taskmark-frontend
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 1
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: S-063
epic: E-017
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
tags: [website, ui, design-system]
created: 2026-07-27
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-27T09:54:28Z
completed_at: 2026-07-27T09:55:28Z
actual_ms: 60000
---
# T-200: Align theme tokens globals and fonts with taskmark-frontend

## Description

Port CSS variables, `globals.css`, and font setup so the website visual baseline matches the board UI.

## Acceptance criteria

- [x] Theme CSS variables match the frontend source of truth.
- [x] Fonts load consistently with the frontend.
- [x] Light/dark (if used) providers can consume the same tokens.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-27T09:54:28Z | prompt | Marco Mendão | Implement E-017 website base Next.js project |
| 1 | 2026-07-27T07:56:00Z | prompt | Marco Mendão | Create epic + stories/tasks for Taskmark website Next.js base sharing frontend UI |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| fa6cb40 | taskmark-website | 2026-07-28T06:19:03Z | Marco Mendão | scaffold taskmark website |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T09:54:28Z | 2026-07-27T09:55:28Z | Delivered with E-017 batch; shared-batch: 1 of 3min by points |
