---
id: T-MM-048b4efc
type: task
title: Add npm publish workflow for taskmark-ui
status: done
priority: high
size: S
points: 3
parent: S-MM-9956e0ef
epic: E-MM-69ccb23d
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
tags: [ui, npm, ci]
created: 2026-09-15
updated: 2026-09-15T11:20:00Z
started_at: 2026-09-15T11:16:00Z
completed_at: 2026-09-15T11:20:00Z
---
# T-MM-048b4efc: Add npm publish workflow for taskmark-ui

## Description

Add a GitHub Actions workflow on `taskmark-ui` that publishes `@taskmark/components` to the public npm registry on `main`.

## Acceptance criteria

- [x] A workflow publishes with `access: public` using `NPM_TOKEN`.
- [x] The job type-checks before publish.
- [x] README documents the `NPM_TOKEN` repository secret.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T11:14:00Z | prompt | Marco Mendão | Taskmark UI should be a public repository and a public library on npm; make the changes needed for that to be true. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T11:16:00Z | 2026-09-15T11:20:00Z | Added a main-branch npm publish workflow with provenance, typecheck, and a missing-token guard. |
