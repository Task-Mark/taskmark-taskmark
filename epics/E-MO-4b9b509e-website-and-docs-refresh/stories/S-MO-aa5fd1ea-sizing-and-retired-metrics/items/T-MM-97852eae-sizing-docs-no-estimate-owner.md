---
id: T-MM-97852eae
type: task
title: Sizing docs state no estimate or owner
status: done
priority: medium
size: XS
points: 1
parent: S-MO-aa5fd1ea
epic: E-MO-4b9b509e
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
tags: [docs, sizing]
created: 2026-08-29
updated: 2026-08-29T11:41:21Z
started_at: 2026-08-29T11:39:40Z
completed_at: 2026-08-29T11:39:55Z
---

# T-MM-97852eae: Sizing docs state no estimate or owner

## Description

The sizing page already uses the static XS–XXL map and does not teach velocity. It still needs an explicit statement that there is no estimate or owner property and that Actual is the sum of closed leaf Work log intervals.

## Acceptance criteria

- [x] Sizing page keeps XS=1, S=3, M=5, L=8, XL=13, XXL=21 with the agreed meanings.
- [x] Docs state there is no estimate or owner property and that Actual is the sum of closed leaf Work log intervals (parents roll up in the UI).
- [x] No live docs page teaches Current Speed, ETA, estimate intensity, or a generated board README changelog.
- [x] `/docs/velocity` and `/docs/readme` still redirect to current pages.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:37:37Z | prompt | Marco Mendão | Review E-MO-4b9b509e; update remaining sizing copy only if it still lags the product. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:39:40Z | 2026-08-29T11:39:55Z | Added no-estimate/owner and Actual-from-work-log copy on sizing. |
