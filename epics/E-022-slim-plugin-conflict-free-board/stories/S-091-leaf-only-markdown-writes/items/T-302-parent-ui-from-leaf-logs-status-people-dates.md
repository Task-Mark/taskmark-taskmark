---
id: T-302
type: task
title: Mostrar logs, estado, pessoas e datas dos pais a partir das folhas
status: done
priority: high
size: L
size_source: suggested
size_basis: [like:T-296]
points: 8
points_source: suggested
estimate_minutes: 80
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:10min/pt]
session_cap_minutes: 480
parent: S-091
epic: E-022
owner: ""
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
updated: 2026-08-28T15:43:42Z
started_at: 2026-08-28T15:40:33Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---

# T-302: Mostrar logs, estado, pessoas e datas dos pais a partir das folhas

## Description

No detalhe de epic/story, Prompt & feedback, Commits e Work log existem só nas
folhas (task/bug). O frontend agrega essas tabelas no pai em tempo de leitura,
sem gravar nada em `epic.md` / `story.md`.

O estado visível do pai deriva só do estado das folhas. Só se escreve `status`
nas folhas; o plugin não actualiza o estado do pai para “acompanhar” o filho.

Há dois papéis: **quem criou** (`reporters` no próprio ficheiro) e **quem
implementou**. Os implementadores do pai são a união dos implementadores das
folhas descendentes — não se escreve `resolvers` no pai.

`started_at`, `updated` e `completed_at` mostrados no pai são inferidos das
folhas (mínimo / máximo / regra de fecho), sem persistir no markdown do pai.

## Acceptance criteria

- [x] Prompt & feedback, Commits e Work log de um pai no UI são a agregação
      das folhas descendentes (com identificação da folha), sem editar o MD do pai
- [x] Estado mostrado no pai é calculado pelas folhas; alterar estado só nas
      folhas não reescreve `status` no ficheiro do pai
- [x] UI distingue criador (reporters do item) de implementadores; no pai os
      implementadores vêm das folhas, não de `resolvers` no ficheiro pai
- [x] `started_at`, `updated` e `completed_at` no detalhe do pai são inferidos
      das folhas (não escritos no frontmatter do pai para este efeito)

## Notes

Complementa [T-296](T-296-ui-query-parents-and-rollups.md) (listas/pontos).
Mapa de sizing deste épico: XS=1, S=3, M=5, L=8, XL=13, XXL=21.

Auditoria 2026-08-28 (só leitura):

- Plugin (`taskmark-cursor/plugins/taskmark`): create/do/commit e `recompute-actuals.py` (`rollup_parent`, shared-batch, `ensure_started_at_from_sessions`) persistem status, datas, rollups, logs e `resolvers` nos pais. Skills críticas: `create-task`, `start-work`, `complete-work`, `sync-status`, `log-commits`.
- UI (`taskmark-frontend`): parse literal (`parse-detail.ts`, `detail-load.ts`, `work-item-detail-body.tsx`). Só `count-leaves.ts` agrega progresso. Epic não mostra Prompt & feedback. Sem camada `derive-*` nem testes.
- Implementação UI proposta: `build-tree.ts` + `derive-work-item.ts` (status, datas, contributors, `aggregatePromptFeedback` / Commits / Work log com origem da folha), integrar em `detail-load.ts` e `build-snapshot.ts`.
- Plugin (T-294/T-295): deixar de escrever nos pais; este item cobre o que o UI passa a mostrar em vez desses writes.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:36:37Z | prompt | Marco Mendão | Logs nas folhas e agregados no UI do pai; estado, implementadores e datas do pai inferidos das folhas, sem alterar documentos pais. |
| 2 | 2026-08-28T12:38:00Z | feedback | Marco Mendão | Exploração: plugin write-through nos pais; frontend read-through literal. T-302 = derive logs/status/people/dates no UI; T-294/T-295 param writes no plugin. |
| 2 | 2026-08-28T15:43:42Z | feedback | Marco Mendão | Implemented and verified as part of E-022; no commits created. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-28T15:40:33Z | 2026-08-28T15:41:12Z | E-022 shared batch: implemented and verified T-302 (8 points); no commit. |
