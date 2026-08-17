---
id: B-013
type: bug
title: "Static build CSS warnings from `first-child` arbitrary variant Tailwind class"
status: done
priority: low
size: XS
size_source: suggested
size_basis: []
points: 1
points_source: suggested
estimate_minutes: 10
actual_minutes: 2
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: E-014
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
tags: [css, tailwind, build]
created: 2026-07-29
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-29T06:37:00Z
completed_at: 2026-07-29T06:39:44Z
actual_ms: 164000
---
# B-013: Static build CSS warnings from `first-child` arbitrary variant Tailwind class

## Description

`taskmark build` prints 16 Lightning CSS warnings. Source is `MarkdownContent` using ``first-child` arbitrary variant:mt-0` / ``last-child` arbitrary variant:mb-0` — optimizer treats `\f` in escaped `first` as a form-feed escape and corrupts the selector.

## Repro steps

1. Run `yarn build` / `taskmark build` from a board.
2. See “Found 16 warnings while optimizing generated CSS” with garbled `:*�-child` selectors.

## Fix criteria

- [x] Replace with stacked variants (`stacked first/last child utilities` / `stacked last-child utilities`) or equivalent valid CSS.
- [x] Production/static build no longer emits those Lightning CSS warnings.

## Notes

Root cause was twofold: (1) Lightning CSS corrupts Tailwind utilities that embed `:first-child` in the class name; (2) staged builds under the board let Tailwind auto-scan board markdown that mentioned those class strings. Fix: `source(none)` + explicit `@source` for the UI package, and a plain `.tm-md > :first-child` CSS reset instead of arbitrary variants. Package bumped to 0.2.3.
## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|-----| d220a7b | taskmark-frontend | 2026-07-29T06:51:55Z | Marco Mendão | add static board build and preview |
| 81dda43 | taskmark-cursor | 2026-07-29T06:51:55Z | Marco Mendão | add board preview and static hosting stubs |
| 6f9db22 | taskmark-taskmark | 2026-07-29T06:51:56Z | Marco Mendão | sync taskmark board |
-------|------|--------|---------|
| 1 | 2026-07-29T06:37:00Z | prompt | Marco Mendão | CSS optimize warnings with garbled :first-child selectors |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T06:37:00Z | 2026-07-29T06:39:44Z | Use [&>*]:first/last stacked variants |
