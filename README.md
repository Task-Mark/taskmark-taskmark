# taskmark-taskmark

Canonical Taskmark board for the multi-repo Taskmark workspace.

This repo’s **root is the board** (`INDEX.md`, `epics/`, …). Product repos (`taskmark-frontend`, `taskmark-cursor`) are listed in `REPOS.md` for commit attribution — do not nest another `taskmark/` folder here, and do not copy the board into product repos.

## Local board UI

```bash
npm install
npx taskmark serve
```

Opens http://localhost:8275 (package `@taskmark/ui`). Or `npm run serve` / `npm start` (`start` skips opening a browser).

## Deploy on Vercel (Node)

1. Import this repo in Vercel.
2. Framework Preset: **Node** (auto-detects root `server.js`).
3. Install Command: `npm install` (default). Leave Build Command empty.
4. Deploy — `server.js` starts `@taskmark/ui` with `TASKMARK_BOARD` set to this repo root.

Optional: set Start Command to `npm start` (`taskmark serve --no-open`) if you override the Node entry.

<!-- taskmark:project-status:begin -->
## Project status

_Last synced: 2026-07-28T15:34:58.543Z_

| Metric | Value |
|--------|-------|
| Total work items | 348 |
| Complete work items | 347 |
| Current speed | 337 (pts/week · 1 active weeks (90d)) |

<!-- taskmark:project-status:end -->

<!-- taskmark:open-work:begin -->
## Open work items

_Last synced: 2026-07-28T15:34:58.543Z_

Stories, tasks, and bugs that are not done, cancelled, or blocked.

| ID | Type | Title | Status | Size | Points | Parent |
|----|------|-------|--------|------|--------|--------|
| T-256 | task | Make board package Vercel-deployable via Node serve | in_progress | M | 3 | E-014 |

<!-- taskmark:open-work:end -->

<!-- taskmark:changelog:begin -->
## Changelog

_Last synced: 2026-07-28T15:34:58.543Z_

Recent meaningful commits on this board repository (excludes sync / housekeeping).

| Date (UTC) | SHA | Author | Message |
|------------|-----|--------|---------|
| 2026-07-28 | `31a2da5` | Marco Mendão | add e-019 documentation epic |
| 2026-07-27 | `a494e58` | Marco Mendão | add e-015 metrics and remove velocity board |
| 2026-07-24 | `8c8d50e` | Marco Mendão | complete t-141 brand hover underline |
| 2026-07-24 | `efa533f` | Marco Mendão | complete t-140 week range dual dropdown |
| 2026-07-24 | `ea2c152` | Marco Mendão | complete e-012 timeframe filters |
| 2026-07-23 | `e6f0170` | Marco Mendão | complete e-011 git identity contributors |
| 2026-07-23 | `767515a` | Marco Mendão | complete t-110 progress bars board |
| 2026-07-23 | `83957ad` | Marco Mendão | complete t-108 t-109 done sort rules |
| 2026-07-23 | `c964895` | Marco Mendão | complete e-010 list search and filters |
| 2026-07-23 | `1245518` | Marco Mendão | complete e-009 list pagination board |
| 2026-07-23 | `bbab1eb` | Marco Mendão | add t-087 date-fns board |
| 2026-07-23 | `ac93736` | Marco Mendão | add t-086 markdown detail board |
| 2026-07-23 | `1cee199` | Marco Mendão | add t-084 t-085 date tooltip board |
| 2026-07-23 | `32e276b` | Marco Mendão | add t-083 sheet children board |
| 2026-07-23 | `ce68818` | Marco Mendão | complete e-006 work items tabs |
| 2026-07-23 | `6201583` | Marco Mendão | add e-009 work items list view epic |
| 2026-07-23 | `dcebe32` | Marco Mendão | complete t-080 t-081 list totals |
| 2026-07-23 | `d5eb379` | Marco Mendão | add t-080 list totals task |
| 2026-07-23 | `6aae4fd` | Marco Mendão | remove unattached story fix b-005 |
| 2026-07-23 | `f3c7b3e` | Marco Mendão | complete s-029 optional hierarchy board |
| 2026-07-23 | `23411cb` | Marco Mendão | add e-007 optional hierarchy board |
| 2026-07-22 | `603c59c` | Marco Mendão | add e-006 list views board |
| 2026-07-21 | `e890d82` | Marco Mendão | add e-005 view work item board |
| 2026-07-21 | `6204471` | Marco Mendão | backfill work logs on done items from velocity |
| 2026-07-21 | `9883b62` | Marco Mendão | sync e-004 timing and points rollup on board |
| 2026-07-21 | `758cd8c` | Marco Mendão | add e-004 speed and estimation epic |
| 2026-07-21 | `95a7951` | Marco Mendão | add b-003 flat board discovery bug |
| 2026-07-21 | `9510b02` | Marco Mendão | add flat taskmark board |

<!-- taskmark:changelog:end -->

<!-- taskmark:contributors:begin -->
## Contributors

People who created or resolved work items on this board (from local git config).

- Marco Mendão <marco.mendao@betacode.tech>

<!-- taskmark:contributors:end -->
