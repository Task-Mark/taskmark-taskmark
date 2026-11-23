---
id: T-MM-8b7b390a
type: task
title: Team presence summaries grouped by project
status: backlog
priority: high
size: M
points: 5
parent: S-MM-6491d502
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, presence]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-8b7b390a: Team presence summaries grouped by project

## Description

Render the AI presence cards from the dashboard payload grouped by project: a section per project with one card per person, reusing `ActorAvatar` and the visual style of `work-presence-feed.tsx`. Cards show the short present-tense sentence with the full paragraph available on open, so each team's current focus reads at a glance.

## Acceptance criteria

- [ ] Each project with presence cards shows a titled group; projects without recent worklogs are omitted.
- [ ] One card per person shows the preview sentence and exposes the full summary.
- [ ] Author and project filters hide non-matching cards and groups.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — AI presence summaries grouped by project/team. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
