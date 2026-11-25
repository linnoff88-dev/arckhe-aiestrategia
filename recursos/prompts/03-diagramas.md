# 03 — Diagramas (Estado Atual + Futuro) em Mermaid

**Objetivo:** gerar o código Mermaid dos diagramas que visualizam a jornada de
transformaçêo de IA de `{empresa}` (atual vs futuro, fluxo de dados, roadmap).

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa (use o inventário tecnológico e as dores, se já gerados):
{pesquisa}

# Tarefa: Gerar diagramas Mermaid (estado atual e futuro)

Com base no inventário e nas dores acima, crie diagramas Mermaid (código válido)
que mostrem a transformaçêo de IA de {empresa}.

## Diagramas obrigatórios

### 1. Arquitetura do estado atual
flowchart mostrando o cenário tecnológico de hoje: fontes de dados, sistemas
centrais, pontos de integraçêo, usuários e gargalos conhecidos (marque os
gargalos com indicador de alerta / cor vermelha).

### 2. Arquitetura do estado futuro (habilitada por IA)
flowchart com a arquitetura-alvo: plataforma de dados unificada, camada de
serviços de IA/ML, aplicações aprimoradas, novas integrações e fluxos de
automaçêo.

### 3. Fluxo de dados
flowchart mostrando como o dado flui pela organizaçêo: ingestêo → processamento
→ armazenamento → analytics → açêo.

### 4. Roadmap de implementaçêo (Gantt)
gantt com as fases (Fundaçêo, Vitórias rápidas, Escala) e durações.

### 5. Arquitetura de integraçêo
flowchart do hub de integraçêo (API gateway, ETL, fila de mensagens).

## Formato de saída
Para cada diagrama: bloco de código Mermaid completo + descriçêo breve +
pontos-chave da transformaçêo + suposições feitas. Use sintaxe Mermaid válida,
nomes consistentes e mantenha legível. Customize ao contexto de {empresa}.
```

## Saída esperada
Markdown com 5 blocos de código Mermaid (atual, futuro, fluxo de dados, Gantt,
integraçêo), cada um com descriçêo. Renderize com eraser.io / `beautiful-mermaid`
(ver `diagramas/README.md`).
