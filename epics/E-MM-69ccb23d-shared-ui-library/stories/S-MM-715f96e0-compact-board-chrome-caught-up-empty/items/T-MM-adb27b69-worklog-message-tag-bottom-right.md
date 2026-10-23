---
id: T-MM-adb27b69
type: task
title: Place the worklog message item tag at the bottom right
status: done
priority: high
size: XS
points: 1
parent: S-MM-715f96e0
epic: E-MM-69ccb23d
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
tags: [ui, worklog]
created: 2026-09-15
updated: 2026-09-16T11:46:46Z
started_at: 2026-09-15T22:11:00Z
completed_at: 2026-09-16T11:46:46Z
---
# T-MM-adb27b69: Place the worklog message item tag at the bottom right

## Description

In each floating worklog message bubble, keep the summary as the main text and move the work-item code tag to the bottom-right corner of the bubble.

## Acceptance criteria

- [x] The worklog footer shows the started date on the left and the item tag on the right.
- [x] The message text is clamped to four lines.
- [x] Clicking the message opens a modal with the full summary.
- [x] The tag still uses the typed badge and title tooltip.
- [x] The layout applies on local, npx static, and Cloud boards.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-16T11:46:46Z | prompt | Marco Mendão | Put the worklog task tag under the message, right-aligned with the date on the left; clamp the text to four lines and open the full message in a modal on click. |
| 2026-09-15T22:48:00Z | prompt | Marco Mendão | Keep the worklog task tag right-aligned, but move it to the top of the bubble. |
| 2026-09-15T22:11:00Z | prompt | Marco Mendão | Put the worklog message task tag at the bottom right of the bubble. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-16T11:44:00Z | 2026-09-16T11:46:46Z | Moved the item tag beside the started date, clamped the summary to four lines, and opened the full message in a modal. |
| Marco Mendão | 2026-09-15T22:48:00Z | 2026-09-15T22:48:00Z | Moved the worklog bubble item tag to the top right. |
| Marco Mendão | 2026-09-15T22:11:00Z | 2026-09-15T22:28:00Z | Moved the worklog bubble item tag to the bottom right. |
