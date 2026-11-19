# 03 — Diagramas (Estado Atual + Futuro) em Mermaid

**Objetivo:** gerar o código Mermaid dos diagramas que visualizam a jornada de
transformação de IA de `{empresa}` (atual vs futuro, fluxo de dados, roadmap).

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa (use o inventário tecnológico e as dores, se já gerados):
{pesquisa}

# Tarefa: Gerar diagramas Mermaid (estado atual e futuro)

Com base no inventário e nas dores acima, crie diagramas Mermaid (código válido)
que mostrem a transformação de IA de {empresa}.

## Diagramas obrigatórios

### 1. Arquitetura do estado atual
flowchart mostrando o cenário tecnológico de hoje: fontes de dados, sistemas
centrais, pontos de integração, usuários e gargalos conhecidos (marque os
gargalos com indicador de alerta / cor vermelha).

### 2. Arquitetura do estado futuro (habilitada por IA)
flowchart com a arquitetura-alvo: plataforma de dados unificada, camada de
serviços de IA/ML, aplicações aprimoradas, novas integrações e fluxos de
automação.

### 3. Fluxo de dados
flowchart mostrando como o dado flui pela organização: ingestão → processamento
→ armazenamento → analytics → ação.

### 4. Roadmap de implementação (Gantt)
gantt com as fases (Fundação, Vitórias rápidas, Escala) e durações.

### 5. Arquitetura de integração
flowchart do hub de integração (API gateway, ETL, fila de mensagens).

## Formato de saída
Para cada diagrama: bloco de código Mermaid completo + descrição breve +
pontos-chave da transformação + suposições feitas. Use sintaxe Mermaid válida,
nomes consistentes e mantenha legível. Customize ao contexto de {empresa}.
```

## Saída esperada
Markdown com 5 blocos de código Mermaid (atual, futuro, fluxo de dados, Gantt,
integração), cada um com descrição. Renderize com eraser.io / `beautiful-mermaid`
(ver `diagramas/README.md`).
