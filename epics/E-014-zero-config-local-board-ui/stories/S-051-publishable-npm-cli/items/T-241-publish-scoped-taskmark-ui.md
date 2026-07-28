---
id: T-241
type: task
title: Publish local UI as scoped package @taskmark/ui
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-154]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-241]
session_cap_minutes: 480
parent: S-051
epic: E-014
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
tags: [frontend, packaging, cli, npm]
created: 2026-07-28
updated: 2026-07-28T09:13:02Z
started_at: 2026-07-28T09:07:14Z
completed_at: 2026-07-28T09:10:14Z
actual_ms: 180000
---
# T-241: Publish local UI as scoped package @taskmark/ui

## Description

Publish the local board UI as npm package **`@taskmark/ui`** with bin **`taskmark`**, so installing it in a Taskmark board/project folder enables `npx taskmark serve` against that folder.

## Acceptance criteria

- [x] Package `name` is `@taskmark/ui` with `publishConfig.access: public`.
- [x] Bin remains `taskmark` (subcommand `serve`).
- [x] Docs show install-in-board-folder: `npm i @taskmark/ui` then `npx taskmark serve` (port 8275).
- [x] Board-ui stub / init docs depend on `@taskmark/ui`, not unscoped `taskmark`.
- [x] Published install stays lean (prebuilt standalone; app build deps are not required at runtime for consumers).

## Notes

Without a local install, `npx -p @taskmark/ui taskmark serve` also works once published.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T09:06:36Z | prompt | Marco Mendão | Create npm package @taskmark/ui installable in taskmark folder for npx taskmark serve |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 31800fc | taskmark-taskmark | 2026-07-28T09:13:02Z | Marco Mendão | log T-241 @taskmark/ui commits |
| b62a48c | taskmark-frontend | 2026-07-28T09:12:29Z | Marco Mendão | publish local ui as @taskmark/ui |
| bce55d8 | taskmark-cursor | 2026-07-28T09:12:29Z | Marco Mendão | point board init at @taskmark/ui |
| bd0fede | taskmark-taskmark | 2026-07-28T09:12:29Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T09:07:14Z | 2026-07-28T09:10:14Z | Publish package as @taskmark/ui; bin taskmark; docs + stub |

