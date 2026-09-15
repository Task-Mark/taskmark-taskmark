---
id: T-MM-3f18de11
type: task
title: Add a local script to bump every product version
status: done
priority: high
size: S
points: 3
parent: S-MM-5fb0e29c
epic: E-MM-d00339e1
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
tags: [release, versioning]
created: 2026-09-15
updated: 2026-09-15T21:45:00Z
started_at: 2026-09-15T21:43:03Z
completed_at: 2026-09-15T21:45:00Z
---
# T-MM-3f18de11: Add a local script to bump every product version

## Description

Add `bump-version.sh` beside the product clones, next to `release.sh` and outside every git repo. A maintainer can set an explicit SemVer or increment patch, minor, or major from the board version. The script writes that SemVer to every product-root `package.json` and the Cursor plugin `plugin.json`. It does not write the changelog, commit, tag, or publish.

## User story

As a maintainer, I run one local script to align every product on a new SemVer when I already know the version I want, without waiting for `/tkmd-version` to collect changelog notes.

## Acceptance criteria

- [x] Workspace-root `bump-version.sh` exists, is executable, and prints usage with `--help`.
- [x] An explicit SemVer argument writes that version to every product-root `package.json` and the Cursor plugin `plugin.json`.
- [x] `--patch`, `--minor`, and `--major` increment from the board `package.json` version.
- [x] `--dry-run` prints the files that would change without writing them.
- [x] The script does not write `CHANGELOG.md`, commit, tag, or publish.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T21:43:03Z | prompt | Marco Mendão | Create a script to bump versions across the projects. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T21:43:03Z | 2026-09-15T21:45:00Z | Added workspace-root bump-version.sh to set or increment the SemVer on every product package.json and the Cursor plugin, with a dry-run mode and no changelog or git writes. |
