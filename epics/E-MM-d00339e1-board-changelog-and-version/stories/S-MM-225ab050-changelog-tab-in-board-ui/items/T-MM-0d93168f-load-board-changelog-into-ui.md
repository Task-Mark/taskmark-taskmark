---
id: T-MM-0d93168f
type: task
title: Load board CHANGELOG.md into live UI and snapshot
status: backlog
priority: high
size: S
points: 3
parent: S-MM-225ab050
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, changelog, snapshot]
created: 2026-08-29
updated: 2026-08-29T17:33:19Z
started_at: null
completed_at: null
---

# T-MM-0d93168f: Load board CHANGELOG.md into live UI and snapshot

## Description

Read `CHANGELOG.md` from the board root (sibling `*-taskmark` or nested `taskmark/`). Expose the markdown on the live board payload and in the static snapshot. Treat missing or whitespace-only files as absent (`null` / omitted), never as an empty tab source. Do not generate or rewrite the file.

## Acceptance criteria

- [ ] Live board load returns changelog markdown when `CHANGELOG.md` exists and has content
- [ ] Missing or whitespace-only `CHANGELOG.md` is represented as absent
- [ ] Static `taskmark-snapshot.json` includes the same present/absent changelog so hosted/static boards match live serve
- [ ] The loader never writes `CHANGELOG.md` or a README changelog

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:33:19Z | prompt | Marco Mendão | Add a frontend tab for the project changelog; if the changelog does not exist, the tab must not exist either. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
