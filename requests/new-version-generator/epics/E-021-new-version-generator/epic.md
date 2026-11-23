---
id: E-021
type: epic
title: New version generator
status: backlog
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 34
points_source: rolled_up
estimate_minutes: 340
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [release, versioning, changelog, readme, plugin]
created: 2026-07-29
updated: 2026-08-28T12:37:43.783Z
started_at: null
completed_at: null
actual_ms: 0
---

# E-021: New version generator

## Goal

Ship a release workflow that bumps versions across linked Taskmark projects and maintains a versioned, end-user-readable changelog in the board README — accumulating work under **Development** until a release promotes it into a numbered version.

## Scope

- Inspect linked product projects (from `REPOS.md`) and their package versions.
- Accept an explicit version from the user, or auto-suggest a suitable semver bump from changes since the last release.
- Apply the chosen version across the relevant project packages.
- Replace the current commit-table README changelog with a versioned changelog.
- While work is in progress, append change notes under a **Development** section.
- On release: move Development contents into the new version section and clear Development.
- Changelog entries must use meaningful end-user language — never raw work-item codes (e.g. `B-009`) or terse commit shorthand like `fix B-009 vercel ui production dep`.

## Out of scope

- Publishing npm packages or creating git tags/GitHub Releases (can follow in a later epic).
- Marketing website release notes pages (README on the board/project is the target).
- Changing product app version display in the UI beyond package.json / release metadata touched by this flow.

## Success metrics

- User can create a new version with one command/skill, with or without supplying a version string.
- All linked versioned packages move to the same release version when appropriate.
- README changelog shows Development + released versions; Development empties after each release.
- A visitor reading the changelog understands what changed without knowing board IDs.

## Stories

- [S-085: Multi-project version bump](stories/S-085-multi-project-version-bump/story.md)
- [S-086: Versioned README changelog with Development bucket](stories/S-086-versioned-readme-changelog/story.md)
- [S-087: Human-readable changelog messages](stories/S-087-human-readable-changelog-messages/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 8b5fdb3 | taskmark-taskmark | 2026-07-29T11:28:26+01:00 | Marco Mendão | add e-021 version generator and b-014 |
| 6da0049 | taskmark-taskmark | 2026-07-29T11:28:54+01:00 | Marco Mendão | update readme dashboard |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
