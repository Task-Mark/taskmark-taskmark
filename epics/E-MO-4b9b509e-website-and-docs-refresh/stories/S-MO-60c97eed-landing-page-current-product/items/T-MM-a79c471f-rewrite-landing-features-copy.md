---
id: T-MM-a79c471f
type: task
title: Rewrite landing features as outcome cards
status: done
priority: high
size: S
points: 3
parent: S-MO-60c97eed
epic: E-MO-4b9b509e
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
tags: [website, landing]
created: 2026-08-29
updated: 2026-08-29T18:51:25Z
started_at: 2026-08-29T18:50:10Z
completed_at: 2026-08-29T18:51:25Z
---

# T-MM-a79c471f: Rewrite landing features as outcome cards

## Description

Replace the technical landing feature inventory (sizing, work logs, leaf-only writes, multi-repo, slash commands) with five outcome cards plus Hierarchical boards as the sixth. Keep site copy in English. Do not mention idle or session-cap velocity. Hero and Purpose stay as they are.

Section heading: `Work that agents can remember — and teams can see`

Section lead: `A markdown board humans and agents share: context, delivery, and release notes without a second tracker.`

Cards (in order):

1. Product memory for agents (`feature-memory`) — Chat is not a backlog. The board is the product context agents read and update — so planning survives the session.
2. Agents report their own work (`feature-agent-log`) — You cannot pre-write every task in an agentic project. As features land, the agent records what it actually did, so the board stays true without a human tax.
3. Everyone on one board (`feature-team`) — People and agents write the same leaves. Status, contributors, and activity roll up so you can see who shipped what.
4. Changelogs users can read (`feature-changelog`) — Done work becomes Keep a Changelog notes for each version — user-facing outcomes, not ticket IDs.
5. Priorities and points that steer delivery (`feature-pace`) — Priority plus a fixed story-point scale sequences work and shows how fast the team is moving — without inventing estimates from the past.
6. Hierarchical boards (`feature-boards`) — Epics, stories, tasks, and bugs as markdown — nested product memory the agent can read and update, without a generated dashboard.

Suggested Lucide icons: Brain, Bot, Users, Newspaper, ListOrdered, FolderTree (keep FolderTree on the sixth). Keep the `feature-boards` anchor. Do not add a git/merge-safe card. Docs and READMEs are out of scope.

## Acceptance criteria

- [x] `taskmark-website/lib/features.ts` lists the six cards above with matching ids, titles, descriptions, and icons
- [x] Features section title and lead match the heading and lead above
- [x] Copy does not mention idle, session-cap, or calibrated velocity
- [x] `feature-boards` remains a stable in-page id
- [x] Hero, Purpose, docs, and READMEs are unchanged

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T18:49:43Z | prompt | Marco Mendão | Cursor plan: rewrite landing features to five outcome cards plus Hierarchical boards; English copy only; no git/merge-safe sixth alternative |
| 2026-08-29T18:50:10Z | prompt | Marco Mendão | Implement this task |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:50:10Z | 2026-08-29T18:51:25Z | Six outcome feature cards with new icons; refreshed section heading and lead; typecheck clean. |
