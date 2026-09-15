---
id: T-MM-1a261ba9
type: task
title: Request contributor summaries from a Cloud overflow menu
status: done
priority: high
size: M
points: 5
parent: S-MM-f998c021
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
tags: [cloud, presence, ui]
created: 2026-09-11
updated: 2026-09-15T22:44:00Z
started_at: 2026-09-11T18:51:00Z
completed_at: 2026-09-11T19:05:43Z
---
# T-MM-1a261ba9: Request contributor summaries from a Cloud overflow menu

## Description

Add a three-dot overflow control beside the Cloud theme toggle. It contains Settings and opens a contributor picker before a member requests one person's work summary. While that summary is generating, show a presence-style message card for the selected person.

## Acceptance criteria

- [x] A three-dot button sits next to the theme toggle, has no heading label, and contains Settings.
- [x] The summarize action opens a modal where the member selects one contributor with recent worklogs.
- [x] A member request regenerates the selected contributor's presence summary without waiting for the 30-minute tick.
- [x] While the summary is generating, the selected contributor shows a presence message skeleton even when the chrome is minimized; the finished preview and full summary replace that card.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T22:44:00Z | prompt | Marco Mendão | Show a skeleton for that contributor while an AI work summary is generating. |
| 2026-09-11T20:20:00Z | prompt | Marco Mendão | Remove dropdown icons, rename summarize to Report Work, show a left-side message skeleton while generating, and confirm before logout. |
| 2026-09-11T19:07:39Z | prompt | Marco Mendão | Add an icon for each action in the three-dot dropdown. |
| 2026-09-11T19:05:43Z | feedback | Marco Mendão | Open a contributor picker before summarizing, move Settings into the three-dot menu, and remove the Board label. |
| 2026-09-11T18:52:31Z | prompt | Marco Mendão | Add a three-dot button beside the theme toggle to request a summary of each contributor's work, and show a summary card while it is generating. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T22:44:00Z | 2026-09-15T22:44:00Z | Kept the presence sheet open with a contributor skeleton while AI summaries generate. |
| Marco Mendão | 2026-09-11T20:18:00Z | 2026-09-11T20:20:00Z | Renamed Report Work, removed menu icons, added generating skeleton in the presence feed, and a logout confirmation dialog. |
| Marco Mendão | 2026-09-11T19:06:30Z | 2026-09-11T19:07:39Z | Added Sparkles and Settings icons to the Cloud three-dot menu actions. |
| Marco Mendão | 2026-09-11T19:03:00Z | 2026-09-11T19:05:43Z | Added a contributor-selection modal, limited manual generation to the selected person, and moved Settings into the unlabeled overflow menu. |
| Marco Mendão | 2026-09-11T18:51:00Z | 2026-09-11T18:59:04Z | Added a Cloud overflow action that requests contributor summaries and streams generating cards until the finished text replaces them. |
