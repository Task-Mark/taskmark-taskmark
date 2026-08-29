---
id: T-MO-d2ec531b
type: task
title: Carry plan diagrams and visuals into created items
status: done
priority: high
size: M
points: 5
parent: S-MO-674a66e5
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [plugin, planning, cursor-plan, visuals]
created: 2026-08-29
updated: 2026-08-29T11:14:10Z
started_at: 2026-08-29T11:09:00Z
completed_at: 2026-08-29T11:14:10Z
---

# T-MO-d2ec531b: Carry plan diagrams and visuals into created items

## Description

Extend `/tkmd-save` so graphics, diagrams, and other visual supports from the
Cursor plan are present on the work items it creates. Place each visual on the
item whose scope it explains (epic/story for overview diagrams; leaf for
step-level figures). Prefer durable board-friendly forms: Mermaid or markdown
image/links that resolve in the board UI, and copy or reference plan-attached
assets when needed—without rewriting existing parents beyond the new files
being created in the same save.

## Acceptance criteria

- [x] The `tkmd-save` skill documents how to find plan visuals (Mermaid, images, canvases, diagram blocks) and which item type receives them.
- [x] When a plan contains diagrams or visual aids, newly created item markdown includes those visuals (embedded or linked) on the matching epic, story, task, or bug.
- [x] Visuals that span multiple leaves are duplicated or linked from each relevant new item, or placed once on the nearest new parent that covers them—documented in the skill.
- [x] Saving a plan with no visuals still succeeds; absence of visuals is not an error.
- [x] No new derived board files; assets live under the board or item paths only as needed for the new items.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:58:33Z | prompt | Marco Mendão | Add `/tkmd-save` after Cursor Plan mode: split the plan into epic/story/task/bug work items and keep plan diagrams/visuals on those items. |
| 2026-08-29T11:09:00Z | prompt | Marco Mendão | `/tkmd-do`: implement every backlog work item under epic E-022. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:09:00Z | 2026-08-29T11:10:14Z | Documented plan visual placement, spanning figures, and no-visuals success in `tkmd-save`. |
