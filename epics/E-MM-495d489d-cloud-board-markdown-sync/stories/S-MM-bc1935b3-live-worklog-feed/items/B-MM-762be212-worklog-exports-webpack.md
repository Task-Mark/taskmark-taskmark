---
id: B-MM-762be212
type: bug
title: Local board 500s because WorklogPanel and flattenWorklogEntries are missing from webpack
status: done
priority: high
size: S
points: 3
parent: S-MM-bc1935b3
epic: E-MM-495d489d
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
tags: [local-ui, webpack, worklog]
created: 2026-09-04
updated: 2026-09-04T15:29:04Z
started_at: 2026-09-04T15:24:15Z
completed_at: 2026-09-04T15:29:04Z
---
# B-MM-762be212: Local board 500s because WorklogPanel and flattenWorklogEntries are missing from webpack

## Description

`taskmark dev` compiles the home page then returns 500. Webpack reports that `flattenWorklogEntries` is not exported from `@taskmark/components/board-model` and `WorklogPanel` is not exported from `@taskmark/components/board`. The local board screen is a server component importing those names from mixed barrels.

## Fix criteria

- [x] Webpack can resolve `flattenWorklogEntries` from `@taskmark/components/board-model`.
- [x] The Worklog view renders `WorklogPanel` without a missing-export compile error.
- [x] `GET /` no longer 500s for that import path.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T15:24:15Z | prompt | Marco Mendão | Local board 500: flattenWorklogEntries and WorklogPanel are not exported to webpack. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-04T15:24:15Z | 2026-09-04T15:29:04Z | Import WorklogPanel via a client module and flattenWorklogEntries from the worklog subpath so webpack keeps the runtime exports. |
