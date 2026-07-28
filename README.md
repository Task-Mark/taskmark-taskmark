# taskmark-taskmark

Canonical Taskmark board for the multi-repo Taskmark workspace.

This repo’s **root is the board** (`INDEX.md`, `epics/`, …). Product repos (`taskmark-frontend`, `taskmark-cursor`) are listed in `REPOS.md` for commit attribution — do not nest another `taskmark/` folder here, and do not copy the board into product repos.

<!-- taskmark:project-status:begin -->
## Project status

_Last synced: 2026-07-28T07:42:10.104Z_

| Metric | Value |
|--------|-------|
| Total work items | 326 |
| Complete work items | 284 |
| Current speed | 337 (pts/week · 1 active weeks (90d)) |

<!-- taskmark:project-status:end -->

<!-- taskmark:open-work:begin -->
## Open work items

_Last synced: 2026-07-28T07:42:10.104Z_

Stories, tasks, and bugs that are not done, cancelled, or blocked.

| ID | Type | Title | Status | Size | Points | Parent |
|----|------|-------|--------|------|--------|--------|
| S-050 | story | Zero-config board binding from env and cwd | backlog | L | 9 | E-014 |
| S-051 | story | Publishable npm CLI for local board UI | backlog | XL | 13 | E-014 |
| S-052 | story | Board init one-command UI launch | backlog | M | 5 | E-014 |
| S-072 | story | Docs information architecture and navigation | backlog | L | 7 | E-019 |
| S-073 | story | Setup and installation guide | backlog | M | 6 | E-019 |
| S-074 | story | Slash commands reference | backlog | XL | 13 | E-019 |
| S-075 | story | Board folder structure | backlog | M | 6 | E-019 |
| S-076 | story | Sizing and story points | backlog | M | 5 | E-019 |
| S-077 | story | Velocity and ETA | backlog | M | 5 | E-019 |
| S-078 | story | README dashboard | backlog | M | 5 | E-019 |
| S-079 | story | Core workflows and related topics | backlog | L | 8 | E-019 |
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
| T-219 | task | Document docs IA and topic outline | backlog | S | 2 | S-072 |
| T-220 | task | Docs shell navigation and section routes | backlog | M | 3 | S-072 |
| T-221 | task | Documentation home and overview page | backlog | S | 2 | S-072 |
| T-222 | task | Install and plugin setup guide | backlog | M | 3 | S-073 |
| T-223 | task | Board init and first-run guide | backlog | M | 3 | S-073 |
| T-224 | task | Commands index page | backlog | S | 2 | S-074 |
| T-225 | task | Document /new-epic, /new-story, and /new-task | backlog | M | 3 | S-074 |
| T-226 | task | Document /start-work and /complete-work | backlog | M | 3 | S-074 |
| T-227 | task | Document /commit-all and /log-commits | backlog | S | 2 | S-074 |
| T-228 | task | Document remaining sync and utility commands | backlog | M | 3 | S-074 |
| T-229 | task | Single-repo and multi-repo board layout | backlog | M | 3 | S-075 |
| T-230 | task | Epic story task file conventions | backlog | M | 3 | S-075 |
| T-231 | task | T-shirt sizes and Fibonacci points guide | backlog | M | 3 | S-076 |
| T-232 | task | Parent rollups and estimate suggestions | backlog | S | 2 | S-076 |
| T-233 | task | Current Speed and ETA documentation | backlog | M | 3 | S-077 |
| T-234 | task | Median minutes-per-point estimate docs | backlog | S | 2 | S-077 |
| T-235 | task | Document README sections and metrics | backlog | M | 3 | S-078 |
| T-236 | task | Document README refresh automation | backlog | S | 2 | S-078 |
| T-237 | task | Work logs, idle caps, and actual minutes | backlog | M | 3 | S-079 |
| T-238 | task | Multi-repo day-to-day workflow | backlog | M | 3 | S-079 |
| T-239 | task | Prompt/feedback and commits logs | backlog | S | 2 | S-079 |

<!-- taskmark:open-work:end -->

<!-- taskmark:changelog:begin -->
## Changelog

_Last synced: 2026-07-28T07:42:10.104Z_

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
