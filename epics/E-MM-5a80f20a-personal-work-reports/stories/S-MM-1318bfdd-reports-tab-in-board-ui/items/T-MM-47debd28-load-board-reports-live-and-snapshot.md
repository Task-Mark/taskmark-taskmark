---
id: T-MM-47debd28
type: task
title: Load board reports into the live UI and the snapshot
status: done
priority: high
size: S
points: 3
parent: S-MM-1318bfdd
epic: E-MM-5a80f20a
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
tags: [frontend, reports, snapshot]
created: 2026-08-31
updated: 2026-08-31T07:09:31Z
started_at: 2026-08-31T07:01:00Z
completed_at: 2026-08-31T07:09:31Z
---

# T-MM-47debd28: Load board reports into the live UI and the snapshot

## Description

Add a loader that reads the `.reports/` directory at the board root, keeps files matching `report-YYYYMMDD.md`, and returns them newest first with their markdown. Model it on the existing changelog loader: whitespace-only files count as absent, a missing directory yields an empty list, and the loader never writes. Expose the same list on the live board payload and in the static snapshot so hosted boards match local serve.

## Acceptance criteria

- [x] The loader returns one entry per report with its date and markdown, sorted newest first
- [x] A missing `.reports/` directory or an empty one yields an empty list rather than an error
- [x] Whitespace-only report files are treated as absent
- [x] Filenames that do not match the report pattern are ignored
- [x] The static snapshot carries the same report list as the live payload
- [x] The loader never writes to the board

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: the board UI must know about every report in the system so a Reports tab can list them. |
| 2026-08-31T06:55:00Z | prompt | Marco Mendão | /tkmd-do E-MM-5a80f20a |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T07:01:00Z | 2026-08-31T07:04:00Z | Added the reports loader plus shared report types, wired them into the static snapshot, and covered the loader with unit tests including impossible dates. |
