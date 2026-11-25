# 02 — Matriz de Dores por Departamento

**Objetivo:** levantar as dores de `{empresa}` por área e apontar onde a IA tem
maior potencial de impacto.

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa:
{pesquisa}

# Tarefa: Matriz de Dores por Departamento

Com base no contexto e na pesquisa acima, crie uma análise de dores organizada
por departamento, em markdown PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
- Dores mais críticas da organizaçêo
- Temas comuns identificados
- Oportunidades de maior impacto para IA

### 2. Matriz de dores por departamento
Para cada departamento relevante, uma tabela:
| Dor | Impacto (A/M/B) | Frequência | Contorno atual | Potencial de soluçêo por IA |

Departamentos: Vendas & Marketing, Operações, Financeiro, RH, Atendimento,
TI & Engenharia. (Use só os que fazem sentido para {empresa}.)

### 3. Dores transversais
Dores que cruzam vários departamentos: silos de comunicaçêo, acesso a dados,
atrasos em aprovações, inconsistência de relatórios.

### 4. Matriz de priorizaçêo (esforço × impacto)
Classifique as dores em:
- Vitórias rápidas (alto impacto, baixo esforço)
- Projetos maiores (alto impacto, alto esforço)
- Tarefas de preenchimento (baixo impacto, baixo esforço)
- Tarefas ingratas (baixo impacto, alto esforço)

### 5. Oportunidades de intervençêo com IA
Para cada dor prioritária: tipo de soluçêo de IA/ML, benefício esperado,
complexidade de implementaçêo, pré-requisitos.

## Formato de saída
- Tabelas markdown com notas de impacto (Alto/Médio/Baixo).
- Específico ao setor de {empresa}.
- Priorize com base na pesquisa; marque suposições.
```

## Saída esperada
Markdown com tabelas de dores por área, dores transversais, a matriz esforço ×
impacto e as oportunidades de IA priorizadas.
