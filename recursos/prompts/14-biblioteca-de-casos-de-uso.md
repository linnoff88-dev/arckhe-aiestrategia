# 14 — Biblioteca de Casos de Uso por Departamento

**Objetivo:** catalogar casos de uso de IA para `{empresa}` por área,
classificados por impacto, viabilidade e prontidêo.

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa / insumos (use dores, cenário tecnológico e setor, se gerados):
{pesquisa}

# Tarefa: Biblioteca de Casos de Uso por Departamento

Com base na análise de dores, no cenário tecnológico e no contexto do setor
acima, crie uma biblioteca de casos de uso de IA organizada por departamento, em
markdown PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
Total de casos, oportunidades de alta prioridade, valor potencial estimado,
pontos de partida recomendados.

### 2. Framework de classificaçêo
- Impacto (Alto/Médio/Baixo)
- Viabilidade (Fácil/Média/Difícil)
- Prontidêo (Pronto / Algum trabalho / Muito trabalho)
- Framework TACO (KPMG) para casos agênticos: **T**arefa (automaçêo),
  **A**nálise, **C**riaçêo, **O**rquestraçêo.

### 3-9. Casos de uso por departamento
Para cada área (Vendas & Marketing, Atendimento, Operações, Financeiro, RH,
TI & Engenharia, Transversais), liste 3-4 casos. Cada caso com:
- Tabela (Categoria TACO | Impacto | Viabilidade | Tempo até valor)
- Descriçêo
- Estado atual (como é feito hoje, dores)
- Soluçêo de IA (abordagem, modelo/ferramenta)
- Valor potencial (com faixas, ex.: +20-30% de conversêo)
- Pré-requisitos
- Ferramentas recomendadas

Use códigos: SM-001 (vendas), CS-001 (atendimento), OP-001 (operações),
FN-001 (financeiro), HR-001 (RH), IT-001 (TI), XF-001 (transversal).

### 10. Matriz resumo
| ID | Caso de uso | Depto | Impacto | Viabilidade | Prioridade |

### 11. Recomendações de implementaçêo
Início rápido (mês 1), Fase 2 (meses 2-3), Fase 3 (meses 4-6).

### 12. Resumo de valor
| Departamento | Casos | Valor anual estimado | Investimento |

## Formato de saída
- Análise detalhada por caso, estrutura consistente.
- Priorize por valor e viabilidade; recomende ferramentas específicas.
```

## Saída esperada
Markdown com casos de uso codificados por área (impacto/viabilidade/TACO),
matriz resumo priorizada e recomendações de implementaçêo por fase.
