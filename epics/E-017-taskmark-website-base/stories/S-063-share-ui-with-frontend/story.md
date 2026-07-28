---
id: S-063
type: story
title: Share UI components and visual interface with frontend
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 8
points_source: rolled_up
estimate_minutes: 110
actual_minutes: 2
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-017
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
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-27T09:54:28Z
completed_at: 2026-07-27T09:56:34Z
actual_ms: 120000
---
# S-063: Share UI components and visual interface with frontend

## User story

As a visitor-facing website developer, I want the same UI components and visual interface language as `taskmark-frontend`, so the Taskmark brand and controls look consistent across the board app and the public site.

## Acceptance criteria

- [x] Shared UI primitives (`components/ui` or equivalent) and `cn`/utility helpers are available in the website project.
- [x] Theme tokens, global styles, and fonts match `taskmark-frontend`.
- [x] Marketing-oriented chrome (e.g. header/footer stubs) uses the same interface patterns as the frontend shell where applicable.

## Tasks

- [T-199: Port shared UI primitives and utility helpers from frontend](items/T-199-port-shared-ui-primitives-and-utility-helpers-from-frontend.md)
- [T-200: Align theme tokens globals and fonts with taskmark-frontend](items/T-200-align-theme-tokens-globals-and-fonts-with-taskmark-frontend.md)
- [T-201: Port shared interface chrome patterns for marketing layout](items/T-201-port-shared-interface-chrome-patterns-for-marketing-layout.md)

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
| 1 | Marco Mendão | 2026-07-27T09:54:28Z | 2026-07-27T09:54:28Z | E-017 shared-batch: 0min rollup (children hold allocation) |
