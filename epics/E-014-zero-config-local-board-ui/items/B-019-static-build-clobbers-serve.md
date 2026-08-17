---
id: B-019
type: bug
title: taskmark build leaves a static .next that serve then runs instead of the app
status: done
priority: high
size: S
size_source: suggested
size_basis: [B-018]
points: 2
points_source: suggested
estimate_minutes: 7
actual_minutes: 10
estimate_source: suggested
estimate_basis: [calibrated:B-018]
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
tags: [frontend, cli, build]
created: 2026-08-17
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-08-17T08:00:00Z
completed_at: 2026-08-17T08:10:00Z
actual_ms: 600000
---
# B-019: taskmark build leaves a static .next that serve then runs instead of the app

## Description

`taskmark build` runs Next with `output: export` in place, so it overwrites the package's `.next` with an export build. `ensureProdNext()` only checked for a `server/` directory, which an export build also has, so the next `taskmark serve` booted that build: every route came back prerendered with the static runtime baked in.

The visible symptom was a CLI that announced `mode: workspace (choose projects in the browser)` while the browser got a prerendered board at `/` and a baked `/setup` → `/` redirect, so the setup wizard was unreachable.

## Repro steps

1. Run `taskmark build` (or `npm run build:static`) from a clone or `npm link`ed install.
2. Run `npx @taskmark/ui` from a folder with no board — the CLI reports workspace mode.
3. `/` returns a prerendered board instead of redirecting to the setup wizard, and `/setup` redirects to `/`.

## Fix criteria

- [x] `serve` treats a `.next` containing `export-detail.json` as unusable and falls back to `dist/prod-next`.
- [x] An in-place `taskmark build` parks the server build and restores it afterwards, on success and on failure.
- [x] Static output is unchanged: `out/index.html` still holds the board.
- [x] Workspace mode reaches the setup wizard; bound mode still serves the board at `/`.

## Notes

`export-detail.json` is the discriminator — Next writes `export-marker.json` for every build but `export-detail.json` only when an export actually ran. When `serve` finds one it deletes the directory and symlinks `dist/prod-next`, so an install left in this state heals itself on the next run.

Staged builds (the package installed under `node_modules`) already built in a copy under the board and were never affected; only clones and `npm link` installs hit this.

Verified: after `taskmark build`, `.next` is still a server build with no `export-detail.json` and no leftover `.next.taskmark-serve`. Workspace mode from `/tmp` gives `/` 307 → `/setup` 200 wizard; bound mode from the board root gives `/` 200, `/board` 200, `/setup` 307 → `/`; `out/index.html` is 2.2 MB of board.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-17T08:00:00Z | prompt | Marco Mendão | npx @taskmark/ui says workspace mode but no setup interface appears |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| e8cba45 | taskmark-frontend | 2026-08-17T09:56:59Z | Marco Mendão | serve board at / and keep static build out of serve |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-17T08:00:00Z | 2026-08-17T08:10:00Z | serve rejects export builds and falls back to dist/prod-next; static build stashes and restores .next |
