---
id: T-219
type: task
title: Document docs IA and topic outline
status: done
priority: medium
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: S-072
epic: E-019
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
tags: [docs, website, documentation]
created: 2026-07-28
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-28T07:43:14Z
completed_at: 2026-07-28T07:51:14Z
actual_ms: 17454
---

# T-219: Document docs IA and topic outline

## Description

Write the documentation information architecture: sections, routes, and cross-links.

## Acceptance criteria

- [x] IA covers setup, commands, structure, sizing, velocity, README, and workflows
- [x] Outline is recorded in Notes or a docs source file

## Notes

Canonical IA: `taskmark-website/lib/docs-nav.ts` (`DOCS_NAV`).

Routes: /docs, /docs/setup, /docs/commands, /docs/structure, /docs/specification, /docs/sizing, /docs/velocity, /docs/readme, /docs/workflows.

Slash command names on the site prefer `/new-*`; mention `create-*` skill names alongside when helpful.


## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T07:40:05Z | prompt | Marco Mendão | Create documentation epic covering setup, commands (/create-epic, /create-task, /create-story, /start-work, /commit-all and others), folder structure, sizing and story points, velocity, README dashboard, and related topics; create stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T07:43:14.000Z | 2026-07-28T07:43:31.454Z | Documented docs IA in lib/docs-nav.ts; shared-batch: 17454 of 480000ms by points |
