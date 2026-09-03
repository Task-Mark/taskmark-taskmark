---
id: T-MM-b596d418
type: task
title: Render the Cloud worklog speedometer with Tabler mood icons
status: done
priority: high
size: M
points: 5
parent: S-MM-0b520ea3
epic: E-MM-495d489d
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
tags: [cloud, ui, gauge, tabler]
created: 2026-09-03
updated: 2026-09-03T21:33:00Z
started_at: 2026-09-03T19:55:00Z
completed_at: 2026-09-03T20:10:00Z
---
# T-MM-b596d418: Render the Cloud worklog speedometer with Tabler mood icons

## Description

Float a speedometer on the left of the Cloud board, opposite the worklog feed. Fill is today's count divided by the 30-day peak. The center uses Tabler icons: `IconMoodSing` at zero, `IconMoodSmile` once work has started, `IconMoodHappy` from 70% of peak, and `IconFlame` from 17:00 local time when today has reached at least 80% of peak. `IconMoodHappy` and `IconFlame` bounce.

## Acceptance criteria

- [x] The speedometer floats on the left of the Cloud board and shows today's work-log count.
- [x] Gauge fill uses today's count over the 30-day peak.
- [x] Zero work logs uses `IconMoodSing`; any work logs below 70% uses `IconMoodSmile`; 70% or more uses `IconMoodHappy`; from 17:00 local time, 80% or more uses `IconFlame`.
- [x] `IconMoodHappy` and `IconFlame` use `animate-bounce`.
- [x] Icons come from Tabler.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T21:33:00Z | prompt | Marco Mendão | On mobile show the work-log gauge in the page body instead of floating. |
| 2026-09-03T21:28:00Z | feedback | Marco Mendão | Past days looked sad because they were scored against a peak set later; check the maths. |
| 2026-09-03T21:23:00Z | prompt | Marco Mendão | Shrink the center icon so it does not hit the gauge, and show smiles for the last 10 days. |
| 2026-09-03T20:09:00Z | feedback | Marco Mendão | Make the speedometer icon larger and put a circular background behind it. |
| 2026-09-03T20:08:00Z | feedback | Marco Mendão | Make the speedometer icon larger and clearly colored. |
| 2026-09-03T20:05:00Z | prompt | Marco Mendão | Enlarge the speedometer, add a caption, end-of-day annoyed icon below 50%, and traffic-light icon colors. |
| 2026-09-03T19:55:00Z | prompt | Marco Mendão | Add a left floating Cloud speedometer for today's work logs with Tabler mood and flame icons. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T21:33:00Z | 2026-09-03T21:33:00Z | Added an inline gauge layout rendered in the page body on mobile. |
| Marco Mendão | 2026-09-03T21:28:00Z | 2026-09-03T21:28:00Z | Scored each history day against its own trailing peak so later records no longer make past days look bad. |
| Marco Mendão | 2026-09-03T21:23:00Z | 2026-09-03T21:23:00Z | Shrunk the center disc and added a 10-day mood row under the gauge. |
| Marco Mendão | 2026-09-03T20:09:00Z | 2026-09-03T20:09:00Z | Enlarged the center icon and sat it on a colored circular disc. |
| Marco Mendão | 2026-09-03T20:08:00Z | 2026-09-03T20:08:00Z | Enlarged the center icon and switched to filled Tabler variants so the traffic-light color reads clearly. |
| Marco Mendão | 2026-09-03T20:05:00Z | 2026-09-03T20:05:00Z | Enlarged the speedometer, added a peak caption, end-of-day annoyed icon, and traffic-light icon colors. |
| Marco Mendão | 2026-09-03T19:55:00Z | 2026-09-03T20:10:00Z | Floated a left Cloud speedometer with Tabler mood and flame icons. |
