# taskmark-taskmark

Canonical Taskmark board for the multi-repo Taskmark workspace.

This repo’s **root is the board** (`INDEX.md`, `epics/`, …). Product repos (`taskmark-frontend`, `taskmark-cursor`) are listed in `REPOS.md` for commit attribution — do not nest another `taskmark/` folder here, and do not copy the board into product repos.

<!-- taskmark:project-status:begin -->
## Project status

_Last synced: 2026-07-28T07:33:42.238Z_

| Metric | Value |
|--------|-------|
| Total work items | 297 |
| Complete work items | 284 |
| Current speed | 337 (pts/week · 1 active weeks (90d)) |

<!-- taskmark:project-status:end -->

<!-- taskmark:open-work:begin -->
## Open work items

_Last synced: 2026-07-28T07:33:42.238Z_

Stories, tasks, and bugs that are not done, cancelled, or blocked.

| ID | Type | Title | Status | Size | Points | Parent |
|----|------|-------|--------|------|--------|--------|
| S-050 | story | Zero-config board binding from env and cwd | backlog | L | 9 | E-014 |
| S-051 | story | Publishable npm CLI for local board UI | backlog | XL | 13 | E-014 |
| S-052 | story | Board init one-command UI launch | backlog | M | 5 | E-014 |
| T-149 | task | Add TASKMARK_BOARD and TASKMARK_MASTER env resolution | backlog | S | 2 | S-050 |
| T-150 | task | Resolve board from cwd layouts | backlog | S | 2 | S-050 |
| T-151 | task | Skip setup wizard when auto-config is valid | backlog | M | 3 | S-050 |
| T-152 | task | Prefer env and cwd over cookies when auto-config present | backlog | S | 2 | S-050 |
| T-153 | task | Configure Next standalone output for packaging | backlog | M | 3 | S-051 |
| T-154 | task | Create publishable package with CLI bin | backlog | L | 5 | S-051 |
| T-155 | task | CLI starts server and opens browser | backlog | M | 3 | S-051 |
| T-156 | task | Document npx and npm start usage | backlog | S | 2 | S-051 |
| T-157 | task | Document one-command UI launch on board init | backlog | M | 3 | S-052 |
| T-158 | task | Optional stub package.json for npm start | backlog | S | 2 | S-052 |

<!-- taskmark:open-work:end -->

<!-- taskmark:changelog:begin -->
## Changelog

_Last synced: 2026-07-28T07:33:42.238Z_

Recent meaningful commits on this board repository (excludes sync / housekeeping).

| Date (UTC) | SHA | Author | Message |
|------------|-----|--------|---------|
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
