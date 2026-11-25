# 09 — Calculadora de ROI & Análise de Custo

**Objetivo:** projetar o ROI das iniciativas de IA de `{empresa}` (eficiência,
receita, risco), com payback e NPV.

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa / insumos (use quick wins e casos de uso, se gerados):
{pesquisa}

# Tarefa: Calculadora de ROI & Análise de Custo

Com base nos quick wins e casos de uso acima, crie uma análise de ROI usando um
framework de criaçêo de valor e benchmarks do setor, em markdown PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
- ROI projetado (Ano 1), payback, NPV (3 anos), principais alavancas, investimento.

### 2. Framework de valor
- Ganhos de eficiência (tempo/custo)
- Aumento de receita (vendas/novas receitas)
- Reduçêo de risco (custos evitados, compliance)
- Valor estratégico (vantagem competitiva)

### 3. Investimento necessário (3 anos)
Tabelas por categoria (tecnologia, implementaçêo, custos contínuos), com
contingência de 15%. Some o total.

### 4. Análise de criaçêo de valor
- Eficiência (iniciativa | métrica | atual | melhorado | economia/ano)
- Receita (iniciativa | métrica | receita/ano)
- Risco (iniciativa | tipo | probabilidade | impacto | custo evitado)

### 5. Cálculos de ROI
- ROI simples: (Benefícios − Investimento) / Investimento × 100
- Payback (meses): Investimento / Benefícios mensais
- NPV 3 anos (tabela ano | benefícios | custos | líquido | fator de desconto |
  VP), usando taxa de desconto de 10%.

### 6. Análise por iniciativa
| Iniciativa | Investimento | Valor ano 1 | ROI | Payback | Prioridade |

### 7. Análise de sensibilidade
Cenários melhor / base / conservador, com premissas, ROI e NPV de cada.

### 8. Benchmarks do setor
| Métrica | Projeçêo da empresa | Média do setor | Quartil superior |

### 9. Linha do tempo de captura de valor
| Marco | Prazo | Valor liberado | Acumulado |

## Formato de saída
- Valores específicos em reais; mostre a metodologia de cálculo.
- Faixas de sensibilidade; deixe as premissas explícitas.
```

## Saída esperada
Markdown com investimento 3 anos, valor por eficiência/receita/risco, ROI +
payback + NPV, sensibilidade e benchmarks.
(Para virar planilha .xlsx, use `templates/roi-calculator.md`.)
