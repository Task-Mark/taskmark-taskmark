---
id: T-302
type: task
title: Show parent logs, status, people, and dates from leaves
status: done
priority: high
size: L
size_source: suggested
size_basis: [like:T-296]
points: 8
points_source: suggested
parent: S-091
epic: E-022
reporters:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [frontend, board, collaboration, rollup]
created: 2026-08-28
updated: 2026-08-28T22:49:03Z
started_at: 2026-08-28T15:40:33Z
completed_at: 2026-08-28T22:49:03Z
---

# T-302: Show parent logs, status, people, and dates from leaves

## Description

In epic/story detail, Prompt & feedback, Commits, and Work log exist only on
leaves (task/bug). The frontend aggregates those tables on the parent at read
time, without writing anything to `epic.md` / `story.md`.

The parent's visible status is derived only from leaf status. `status` is
written only on leaves; the plugin does not update the parent status to
"follow" the child.

There are two roles: **who created** (`reporters` on the item's own file) and
**who implemented**. Parent implementers are the union of descendant leaf
implementers — `resolvers` is not written on the parent.

`started_at`, `updated`, and `completed_at` shown on the parent are inferred
from leaves (min / max / close rule), without persisting them on parent
markdown.

## Acceptance criteria

- [x] Prompt & feedback, Commits, and Work log for a parent in the UI are the
      aggregation of descendant leaves (with leaf identification), without
      editing the parent's markdown
- [x] Status shown on the parent is computed from leaves; changing status only
      on leaves does not rewrite `status` in the parent file
- [x] The UI distinguishes creator (item reporters) from implementers; on the
      parent, implementers come from leaves, not from `resolvers` on the parent
      file
- [x] `started_at`, `updated`, and `completed_at` on parent detail are inferred
      from leaves (not written to parent frontmatter for this purpose)

## Notes

Complements [T-296](T-296-ui-query-parents-and-rollups.md) (lists/points).
Sizing map for this epic: XS=1, S=3, M=5, L=8, XL=13, XXL=21.

Audit 2026-08-28 (read-only):

- Plugin (`taskmark-cursor/plugins/taskmark`): create/do/commit and `recompute-actuals.py` (`rollup_parent`, shared-batch, `ensure_started_at_from_sessions`) persist status, dates, rollups, logs, and `resolvers` on parents. Critical skills: `create-task`, `start-work`, `complete-work`, `sync-status`, `log-commits`.
- UI (`taskmark-frontend`): literal parse (`parse-detail.ts`, `detail-load.ts`, `work-item-detail-body.tsx`). Only `count-leaves.ts` aggregates progress. Epic does not show Prompt & feedback. No `derive-*` layer or tests.
- Proposed UI implementation: `build-tree.ts` + `derive-work-item.ts` (status, dates, contributors, `aggregatePromptFeedback` / Commits / Work log with leaf origin), integrate in `detail-load.ts` and `build-snapshot.ts`.
- Plugin (T-294/T-295): stop writing to parents; this item covers what the UI now shows instead of those writes.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:36:37Z | prompt | Marco Mendão | Logs on leaves, aggregated in the parent UI; parent status, implementers, and dates inferred from leaves, without changing parent documents. |
| 2 | 2026-08-28T12:38:00Z | feedback | Marco Mendão | Exploration: plugin write-through on parents; frontend literal read-through. T-302 = derive logs/status/people/dates in the UI; T-294/T-295 stop plugin writes. |
| 2 | 2026-08-28T15:43:42Z | feedback | Marco Mendão | Implemented and verified as part of E-022; no commits created. |
| 3 | 2026-08-28T22:45:00Z | prompt | Marco Mendão | Remove Est and Owner; derive Actual exclusively from Work log intervals on leaves. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-28T15:40:33Z | 2026-08-28T15:41:12Z | E-022 shared batch: implemented and verified T-302 (8 points); no commit. |
| 2 | Marco Mendão | 2026-08-28T22:45:00Z | 2026-08-28T22:49:03Z | Removed estimate/owner from the UI model and derived Actual from closed leaf Work log intervals. |
