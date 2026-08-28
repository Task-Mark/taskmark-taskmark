---
id: B-014
type: bug
title: Board crashes when WorkItemSheet Suspense falls back without provider
status: done
priority: high
size: S
size_source: suggested
size_basis: [B-007]
points: 2
points_source: suggested
estimate_minutes: 25
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:12min/pt]
session_cap_minutes: 480
parent: E-005
epic: E-005
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
tags: [dashboard, frontend, sheet, suspense, bug]
created: 2026-07-29
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-29T07:30:00Z
completed_at: 2026-07-29T07:30:44Z
actual_ms: 44000
---

# B-014: Board crashes when WorkItemSheet Suspense falls back without provider

## Description

`WorkItemSheetProvider` wraps `WorkItemSheetProviderInner` (which calls `useSearchParams`) in `React.Suspense` with `fallback={children}`. While search params are pending, list children such as `ViewWorkItemButton` render **outside** the sheet context and throw `useWorkItemSheet must be used within WorkItemSheetProvider`, causing `GET /board` 500.

## Repro steps

1. Open the local board UI at `/board` (no epic selected is enough).
2. Observe a 500 / error overlay referencing `useWorkItemSheet`.

## Fix criteria

- [x] Suspense fallback still provides sheet context (or otherwise does not render `ViewWorkItemButton` without a provider).
- [x] `/board` loads without throwing `useWorkItemSheet must be used within WorkItemSheetProvider`.
- [x] View buttons still open the detail sheet after hydration.

## Notes

Root cause is fallback=`children` bypassing `WorkItemSheetContext.Provider`.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T07:30:00Z | prompt | Marco Mendão | Fix useWorkItemSheet must be used within WorkItemSheetProvider error on /board |
| 2 | 2026-07-29T07:30:44Z | feedback | Marco Mendão | Fixed provider Suspense fallback so ViewWorkItemButton always has context |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 8b5fdb3 | taskmark-taskmark | 2026-07-29T11:28:26+01:00 | Marco Mendão | add e-021 version generator and b-014 |
| 6da0049 | taskmark-taskmark | 2026-07-29T11:28:54+01:00 | Marco Mendão | update readme dashboard |
| 38d75cf | taskmark-frontend | 2026-07-29T11:28:25+01:00 | Marco Mendão | fix sheet suspense fallback and hide paths |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T07:30:00Z | 2026-07-29T07:30:44Z | Fixed Suspense fallback to wrap children in WorkItemSheetContext.Provider |
