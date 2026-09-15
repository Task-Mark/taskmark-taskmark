---
id: T-MM-d661ee92
type: task
title: Configure @taskmark/components for public npm
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
tags: [ui, npm]
created: 2026-09-15
updated: 2026-09-15T11:20:00Z
started_at: 2026-09-15T11:16:00Z
completed_at: 2026-09-15T11:20:00Z
---
# T-MM-d661ee92: Configure @taskmark/components for public npm

## Description

Mark the shared UI package as a public scoped library: license, repository metadata, `publishConfig.access: public`, and install docs for npm.

## Acceptance criteria

- [x] `package.json` is not private, has MIT license, GitHub repository fields, and `publishConfig.access: public`.
- [x] LICENSE and README explain `npm install @taskmark/components`.
- [x] Workspace consumers may keep the `file:` dependency for local development.

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
| Marco Mendão | 2026-09-15T11:16:00Z | 2026-09-15T11:20:00Z | Added public npm metadata, MIT license, and install docs while leaving sibling file: consumers unchanged. |
