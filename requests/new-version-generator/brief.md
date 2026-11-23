---
id: R-new-version-generator
type: request
title: New version generator
status: shelved
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-29
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - release
  - versioning
  - changelog
  - readme
  - plugin
aliases:
  - E-021
source_meetings: []
links: []
---

# New version generator

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

## Done when

- User can create a new version with one command/skill, with or without supplying a version string.
- All linked versioned packages move to the same release version when appropriate.
- README changelog shows Development + released versions; Development empties after each release.
- A visitor reading the changelog understands what changed without knowing board IDs.

## Out of scope

- Publishing npm packages or creating git tags/GitHub Releases (can follow in a later epic).
- Marketing website release notes pages (README on the board/project is the target).
- Changing product app version display in the UI beyond package.json / release metadata touched by this flow.

## Open questions

_None yet._
