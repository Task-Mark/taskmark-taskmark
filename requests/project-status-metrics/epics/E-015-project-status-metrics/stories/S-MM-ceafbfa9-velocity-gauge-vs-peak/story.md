---
id: S-MM-ceafbfa9
type: story
title: Velocity gauge versus historical peak
status: backlog
priority: medium
size: null
points: null
parent: E-015
epic: E-015
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, metrics, velocity, ui]
created: 2026-08-30
updated: 2026-08-30T06:51:01Z
started_at: null
completed_at: null
---

# S-MM-ceafbfa9: Velocity gauge versus historical peak

## User story

As a project lead looking at the board metrics strip, I want a velocity gauge that shows Current Speed against the highest that same speed has ever been, so I can see at a glance whether the project is running at its historical peak or slower.

## Acceptance criteria

- [ ] The metrics strip includes a Velocity card with a notch-based arc gauge (Bklit Gauge), not a hand-rolled donut SVG.
- [ ] The gauge fill (0–100) is current Current Speed divided by the historical peak of that same 90-day weekly average; the center label is the current speed in pts/week.
- [ ] The scale maximum is the peak Current Speed across past and present (never lower than the value shown now).
- [ ] Styling matches the retro board: hard black card chrome, sharp notches, `#C4A1FF` tones, readable in light and dark.
- [ ] Empty boards show an empty track and a clear empty state instead of a fake peak.
