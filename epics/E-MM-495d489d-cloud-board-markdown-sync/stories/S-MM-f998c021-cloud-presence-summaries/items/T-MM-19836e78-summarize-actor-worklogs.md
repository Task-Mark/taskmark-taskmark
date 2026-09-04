---
id: T-MM-19836e78
type: task
title: Summarize each actor's new worklogs with LLM fallback
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
tags: [api, llm, presence]
created: 2026-09-03
updated: 2026-09-04T08:25:30Z
started_at: 2026-09-03T21:56:00Z
completed_at: 2026-09-03T22:02:00Z
---
# T-MM-19836e78: Summarize each actor's new worklogs with LLM fallback

## Description

For each actor with new worklogs in the tick window, produce a verbose present-tense English status from that person's last ten stored worklogs. Call an OpenAI-compatible Chat Completions API using `OPENAI_API_KEY` and optional `OPENAI_BASE_URL` / `OPENAI_MODEL` (default `gpt-4o-mini`). Prompt with actor name, item titles, and worklog summaries. Strip quotes and item ids from the model output. If the key is missing or the call fails, fold the last ten titles and summaries into an extractive fallback so local Cloud still works.

## Acceptance criteria

- [x] Each actor with new events in the window gets a verbose English present-tense status (two to four sentences) drawn from their last ten worklogs, not a list of item ids.
- [x] Optional `OPENAI_API_KEY`, `OPENAI_BASE_URL`, and `OPENAI_MODEL` configure the call; default model is `gpt-4o-mini`.
- [x] Missing key or a failed model call uses the extractive fallback from the last ten worklogs.
- [x] A failed summary for one actor does not drop other actors' cards or fail the activity GET.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T08:25:30Z | prompt | Marco Mendão | Make the AI summary more verbose and base it on the person's last ten worklogs. |
| 2026-09-03T21:56:00Z | prompt | Marco Mendão | Cursor plan: summarize each actor's new worklogs with an LLM and extractive fallback. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-04T08:25:00Z | 2026-09-04T08:25:30Z | Summarized each person from their last ten worklogs in two to four sentences. |
| Marco Mendão | 2026-09-03T21:56:00Z | 2026-09-03T22:02:00Z | Added OpenAI-compatible summaries with extractive fallback. |
