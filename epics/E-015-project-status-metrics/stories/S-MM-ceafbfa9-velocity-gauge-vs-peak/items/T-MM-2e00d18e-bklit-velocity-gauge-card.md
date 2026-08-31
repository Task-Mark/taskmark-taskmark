---
id: T-MM-2e00d18e
type: task
title: Add Bklit velocity gauge card to the metrics strip
status: done
priority: medium
size: L
points: 8
parent: S-MM-ceafbfa9
epic: E-015
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
tags: [frontend, metrics, ui]
created: 2026-08-30
updated: 2026-08-30T20:03:43Z
started_at: 2026-08-30T06:57:15Z
completed_at: 2026-08-30T07:06:06Z
---

# T-MM-2e00d18e: Add Bklit velocity gauge card to the metrics strip

Register `@bklit` in `components.json` and install `@bklit/gauge-chart` via shadcn into `components/charts/`. Wrap `Gauge` in `VelocityGauge`: fill is current/peak × 100, `centerValue` is Current Speed, label `pts / week`. Retro overrides only on the wrapper: sharp rectangular notches, `#EADFFE`→`#C4A1FF` gradient, light-lilac track (not `--border` black), low `minWidth` so a 4-column strip does not overflow. Put a Velocity card on `ProjectStatusMetricsStrip` with existing neo-brutalism chrome. Import from `@/components/charts/gauge`.

## Acceptance criteria

- [x] `@bklit/gauge-chart` is installed as source; no custom donut SVG for this metric.
- [x] Metrics strip shows a Velocity card on live and static boards; grid is `1 / 2 / 4` columns.
- [x] Gauge fill tracks current vs peak; center shows current pts/week; subtitle names the peak and its ISO week when present.
- [x] Empty data: empty track and “No completed points yet” (or equivalent), no invented peak.
- [x] Light and dark modes keep `#C4A1FF` tones and `font-head` on the center value; `npm run lint` passes.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-30T06:51:01Z | prompt | Marco Mendão | Cursor plan: use the Bklit notch gauge (not a custom SVG) for project velocity vs historical peak, retro Taskmark styling and #C4A1FF, as a new metrics-strip card. |
| 2026-08-30T06:57:15Z | prompt | Marco Mendão | /tkmd-do S-MM-ceafbfa9 e S-MM-0ae91e44 |
| 2026-08-30T20:03:43Z | prompt | Marco Mendão | The gauge is too big; make it wider and shorter so every metrics card looks proportional. |
| 2026-08-30T20:03:43Z | feedback | Marco Mendão | Velocity now uses the Bklit linear notch track (`orientation="linear"`, 18px tall, label above), because the arc orientation sizes on min(width, height) and cannot stay short in a strip card. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-30T06:57:15Z | 2026-08-30T07:06:06Z | Bklit Gauge velocity card vs peak in the metrics strip |
| Marco Mendão | 2026-08-30T19:58:00Z | 2026-08-30T20:03:43Z | Reshaped the velocity gauge as a wide, short linear notch track |
