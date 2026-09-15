---
id: B-MM-7587cadf
type: bug
title: Vercel website build cannot resolve @taskmark/components
status: done
priority: high
size: S
points: 3
parent: E-MO-4b9b509e
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
tags: [website, vercel, npm]
created: 2026-09-15
updated: 2026-09-15T23:35:56Z
started_at: 2026-09-15T23:26:00Z
completed_at: 2026-09-15T23:35:56Z
---
# B-MM-7587cadf: Vercel website build cannot resolve @taskmark/components

## Description

The public website Vercel build fails with `Module not found: Can't resolve '@taskmark/components'` from `board-visual.tsx`. The website `package.json` points at `file:../taskmark-ui`, which exists only in the local multi-repo workspace. Vercel clones `taskmark-website` alone, so that sibling path is missing.

## User story

As a visitor, I want the public website to deploy on Vercel so landing and docs stay online after a release.

## Fix criteria

- [x] `taskmark-website` depends on the published `@taskmark/components` SemVer, not a sibling `file:` path.
- [x] The website Next config does not assume a sibling `taskmark-ui` checkout.
- [x] `npm install` and `npm run build` succeed in a standalone website clone.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:26:00Z | prompt | Marco Mendão | Vercel website build cannot resolve `@taskmark/components` from the landing board visual. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T23:26:00Z | 2026-09-15T23:35:56Z | Switched the website to published `@taskmark/components@1.2.0` and made Next config work without a sibling UI checkout. |
