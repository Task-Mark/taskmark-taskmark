---
id: B-017
type: bug
title: npx taskmark runs an unrelated npm package instead of the board UI
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:B-017]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 7
estimate_source: suggested
estimate_basis: [calibrated:B-017]
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
tags: [frontend, cli, npm, packaging]
created: 2026-08-17
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-08-17T07:36:10Z
completed_at: 2026-08-17T07:44:08Z
actual_ms: 478000
---

# B-017: npx taskmark runs an unrelated npm package instead of the board UI

## Description

`npx taskmark` never reaches our CLI. `taskmark` is the **bin name** inside `@taskmark/ui`, not a package name, and an unrelated package called `taskmark` (1.0.2, `github.com/aitorllj93/taskmark`, "The Markdown Tasks specification") already exists on the registry. With no local or global install, npx resolves that foreign package, so no board UI and no project picker ever start.

Two follow-on problems make global use fail even with the right name:

- Local `package.json` was on `0.2.5` while the registry already had `0.2.6`, so the workspace-mode work (T-277, T-278) could never publish.
- `npx @taskmark/ui` pulls the published tarball, which predates smart-default/workspace mode.

## Repro steps

1. From any folder with no `@taskmark/ui` installed, run `npx taskmark`.
2. npm fetches the unrelated `taskmark` package; the Taskmark UI and project picker never appear.

## Fix criteria

- [x] Global invocation documented as `npx @taskmark/ui` (bin `taskmark`), with an explicit warning that bare `npx taskmark` is a different package.
- [x] Package version bumped past the published `0.2.6` so the workspace-mode work is releasable.
- [ ] A globally linked build exposes `taskmark` on PATH and starts workspace mode from a non-board folder.
- [x] Production (prebuilt `next start`) path verified to render the setup / project picker, not a bound board.
- [x] README documents local install, global link, and publish paths.

## Notes

Root cause was twofold. `taskmark` is a bin name, not a package: the registry package `taskmark@1.0.2` (`github.com/aitorllj93/taskmark`) is unrelated, so `npx taskmark` never ran our CLI. Version was also level with the published `0.2.6`, so nothing could ship — bumped to `0.3.0`.

Second, real defect: with a board resolvable at build time, `/setup` was **prerendered** with a baked `redirect("/board")`. In workspace mode the prebuilt server then looped `/` → `/setup` → `/board` → `/setup`, so the picker never rendered even when mode detection was correct (dev mode hid this because it never prerenders). Fixed with `export const dynamic = "force-dynamic"` on `/setup`.

Fixing that surfaced two pre-existing `taskmark build` failures, both now fixed in `scripts/build-static.mjs`:

- The API stash renamed `app/api` → `app/api.staticbak`, still inside `app/`, so Next routed it and rejected its `force-dynamic`. Backup now parks in `.taskmark-build/`.
- `output: "export"` rejects `force-dynamic` on `/board` and `/setup`. Next only accepts a literal (a `process.env` ternary fails with `Unsupported node type "ConditionalExpression"`), so the static build now swaps the literal to `force-static` and restores the sources afterwards.

Verified from `/tmp` with the prebuilt server: `/` → `/setup` (200, wizard with Browse / Find projects); with a saved master cookie → `/board` (200) with `projectId` select and Add project. `taskmark build` produces a static export again.

`npm link` was not run — it changes the machine's global PATH, so it is left to the user.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-17T07:36:10Z | prompt | Marco Mendão | npx taskmark does not show the application with the project picker |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-17T07:36:10Z | 2026-08-17T07:44:08Z | Fixed prerendered /setup redirect loop, bumped to 0.3.0, documented npx @taskmark/ui, and repaired static export stash + force-dynamic swap |
