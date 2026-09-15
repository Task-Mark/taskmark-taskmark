---
id: B-MM-3667b619
type: bug
title: Local UI build fails type-checking shared Skeleton refs
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
tags: [frontend, typescript, npm]
created: 2026-09-15
updated: 2026-09-15T17:54:23Z
started_at: 2026-09-15T17:52:05Z
completed_at: 2026-09-15T17:54:23Z
---
# B-MM-3667b619: Local UI build fails type-checking shared Skeleton refs

## Description

`@taskmark/ui` `next build` (including `prepack` / `npm publish`) type-checks the sibling `@taskmark/components` sources. Those sources pick up a second `@types/react` from `taskmark-ui/node_modules`, so `Skeleton` props `ref` does not match the JSX `div` type and the build fails.

## User story

As a maintainer, I publish `@taskmark/ui` from the local workspace so `npm run build` type-checks the shared UI against one React type package.

## Fix criteria

- [x] `npm run build` in `taskmark-frontend` completes type-check with the local `file:` `@taskmark/components` checkout.
- [x] Shared UI components still transpile from the sibling package.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T17:52:05Z | prompt | Marco Mendão | `npx`/`npm` publish of `@taskmark/ui` fails type-checking `skeleton.tsx` because two `@types/react` copies disagree on `ref`. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T17:52:05Z | 2026-09-15T17:54:23Z | Imported ComponentProps from react in Skeleton so Next type-check no longer mixes two @types/react copies. |
