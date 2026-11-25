# 08 — Consolidaçêo de Licenças

**Objetivo:** achar oportunidades de consolidar licenças de software e reduzir
custos em `{empresa}`.

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa / insumos (use inventário e comparaçêo de fornecedores, se gerados):
{pesquisa}

# Tarefa: Recomendações de Consolidaçêo de Licenças

Com base no inventário e na comparaçêo de fornecedores acima, identifique
oportunidades de consolidar licenças de software e cortar custos, em markdown
PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
- Economia potencial total identificada
- Número de oportunidades de consolidaçêo
- Complexidade de implementaçêo
- Ações prioritárias recomendadas

### 2. Cenário atual de licenças
Inventário (tabela: Categoria | Ferramenta | Fornecedor | Tipo de licença |
Usuários | Custo anual | Data de renovaçêo) e listagem por categoria
(produtividade, dev/DevOps, analytics/BI, CRM/vendas, segurança, IA/automaçêo).

### 3. Oportunidades de consolidaçêo
Para cada oportunidade: estado atual (tabela de ferramentas), consolidaçêo
proposta (para qual ferramenta, justificativa, complexidade de migraçêo) e
análise de economia (custo anual, overhead admin, treinamento → economia total)
e plano de implementaçêo.

### 4. Análise de sobreposiçêo
- Funcionalidade redundante (capacidade | ferramentas que a oferecem |
  ferramenta única recomendada)
- Licenças subutilizadas (compradas vs usuários ativos vs utilizaçêo vs açêo)

### 5. Oportunidades de acordo corporativo (EA)
Candidatos a EA e recomendações de bundle (ex.: Microsoft 365, Google Workspace).

### 6. Consolidaçêo de ferramentas de IA
Ferramentas de IA atuais e o stack de IA recomendado (camada | ferramenta
recomendada | substitui | economia).

### 7. Resumo de economia
Por categoria (gasto atual | proposto | economia | % de reduçêo) e por janela de
tempo (0-3, 3-6, 6-12 meses).

### 8. Roadmap de implementaçêo
Fase 1 (quick wins, 0-3 meses), Fase 2 (3-6 meses), Fase 3 (consolidações
maiores, 6-12 meses), com economia por açêo.

## Formato de saída
- Valores em reais onde possível; priorize por economia.
- Inclua complexidade, dependências e riscos; recomendações acionáveis.
```

## Saída esperada
Markdown com inventário de licenças, oportunidades de consolidaçêo com economia
estimada, análise de sobreposiçêo e roadmap de cortes priorizado.
