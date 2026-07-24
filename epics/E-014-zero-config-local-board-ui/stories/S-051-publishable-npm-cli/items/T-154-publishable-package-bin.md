---
id: T-154
type: task
title: Create publishable package with CLI bin
status: backlog
priority: high
size: L
size_source: suggested
size_basis: [T-153]
points: 5
points_source: suggested
estimate_minutes: 75
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-051
epic: E-014
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, packaging, cli, npm]
created: 2026-07-24
updated: 2026-07-24T17:39:50.198Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-154: Create publishable package with CLI bin

## Description

Create the publishable package layout (working name `@taskmark/ui`) with a `bin` entry that points at a Node CLI, packages the prebuilt server artifact, and can be installed via npm/`npx`.

## Acceptance criteria

- [ ] Package has a `bin` (e.g. `taskmark` or `taskmark-ui`) executable from PATH after install.
- [ ] Published/packed contents include the prebuilt server needed to run without a source checkout.
- [ ] Package `name` / scope decision is recorded in package.json and docs (placeholder OK until publish).

## Notes

Final npm name may be `@taskmark/ui` or `taskmark-ui` depending on registry availability.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
