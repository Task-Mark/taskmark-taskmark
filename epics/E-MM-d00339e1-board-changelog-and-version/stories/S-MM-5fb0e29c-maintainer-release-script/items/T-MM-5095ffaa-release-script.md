---
id: T-MM-5095ffaa
type: task
title: Add a local script to push repos and publish npm packages
status: done
priority: high
size: M
points: 5
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
tags: [release, npm, git]
created: 2026-09-15
updated: 2026-09-15T21:10:00Z
started_at: 2026-09-15T16:54:00Z
completed_at: 2026-09-15T16:58:00Z
---
# T-MM-5095ffaa: Add a local script to push repos and publish npm packages

## Description

Add `release.sh` beside the product clones, outside every git repo and outside the Cursor plugin. After `/tkmd-version`, the maintainer runs it locally. It reads the SemVer from the board `package.json`, refreshes local file dependencies, verifies products, commits remaining dirty product roots, pushes each product repo (and a matching `v*` tag), ensures npm login, asks for one 2FA code, publishes `@taskmark/components` then `@taskmark/ui` (rewriting the local `file:` dependency to that SemVer for the publish pack only).

## User story

As a maintainer, I run one script as the last release step so git remotes and npm stay on the version already cut on disk.

## Acceptance criteria

- [x] Workspace-root `release.sh` exists, is executable, and prints usage with `--help`.
- [x] The Cursor plugin does not ship or install a release script.
- [x] `--dry-run` prints push and publish steps without contacting remotes or the registry.
- [x] Dirty git roots are committed with `cut {version}` after checks and before push; `.env` and credential files stay uncommitted.
- [x] npm login runs only when `npm whoami` fails; otherwise a 2FA prompt is enough for publish.
- [x] `@taskmark/ui` is packed with `@taskmark/components` at the released SemVer, not `file:../taskmark-ui`.
- [x] Publishing aborts when a manifest still points a runtime dependency at a workspace path.
- [x] After publishing, the released `@taskmark/ui` is installed from npm and proven to build a board snapshot.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T16:54:00Z | prompt | Marco Mendão | Create a release script that publishes all npm packages and pushes every repo. Last step after a new version. npm login if needed, then ask for a 2FA code for publish. |
| 2026-09-15T16:59:00Z | prompt | Marco Mendão | The release script must not live in the Cursor plugin. Put it outside every product repo as an internal deploy tool. |
| 2026-09-15T17:00:00Z | feedback | Marco Mendão | Keep it next to the clones as `./release.sh`. Default workspace is the script directory. |
| 2026-09-15T20:37:36Z | prompt | Marco Mendão | Make the release script refresh internal dependencies to the release version and verify that every product completes its checks before push or publish. |
| 2026-09-15T20:43:59Z | prompt | Marco Mendão | Make ./release.sh commit dirty product repos instead of aborting. |
| 2026-09-15T21:00:00Z | prompt | Marco Mendão | A published CLI version broke board sync because it shipped a workspace path dependency. Stop that from reaching npm again. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T16:54:00Z | 2026-09-15T16:58:00Z | Added plugin scripts/release.sh to push product repos, tag the board SemVer, npm login if needed, and publish both public packages with one OTP. |
| Marco Mendão | 2026-09-15T16:59:00Z | 2026-09-15T17:00:00Z | Moved release.sh to the workspace parent of all clones; removed it from the plugin package and the local plugin install. |
| Marco Mendão | 2026-09-15T20:32:00Z | 2026-09-15T20:37:36Z | Added local file-dependency refresh with lockfile preservation, release-version validation, pre-push product checks, and a network-free dry run. |
| Marco Mendão | 2026-09-15T20:43:00Z | 2026-09-15T20:43:59Z | Commit dirty product roots after checks with a one-line cut message, skipping env and credential files. |
| Marco Mendão | 2026-09-15T21:00:00Z | 2026-09-15T21:10:00Z | Refuse to publish manifests that still reference workspace paths, and install the released package from npm afterwards to confirm it can build a board snapshot. |
