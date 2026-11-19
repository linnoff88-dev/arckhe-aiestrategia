# 07 — Comparação de Fornecedores & Construir vs Comprar

**Objetivo:** comparar fornecedores de IA e decidir construir vs comprar para os
casos de uso de `{empresa}`.

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa / insumos (use inventário e casos de uso, se gerados):
{pesquisa}

# Tarefa: Comparação de Fornecedores & Construir vs Comprar

Com base no inventário e nos casos de uso acima, crie uma comparação de
fornecedores e análise construir vs comprar, em markdown PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
- Recomendações de fornecedor por categoria
- Recomendações construir vs comprar
- Custo total de propriedade estimado
- Fatores críticos de decisão

### 2. Comparação de plataformas de IA
Plataformas corporativas (tabela: Fornecedor | Forças | Fraquezas | Melhor para
| Modelo de preço): Microsoft Azure AI, Google Cloud AI, AWS AI, OpenAI, Claude
(Anthropic).
Mais tabelas por categoria: processamento de documentos, IA conversacional,
analytics & BI, automação de processos (colunas: Recursos | Integração | Preço |
Aderência).

### 3. Framework construir vs comprar
Matriz de decisão por caso de uso:
| Fator | Peso | Nota construir | Nota comprar |
|---|---|---|---|
| Tempo até valor | 25% | | |
| Custo total (3 anos) | 20% | | |
| Necessidade de customização | 15% | | |
| Valor estratégico | 15% | | |
| Capacidade interna | 10% | | |
| Esforço de manutenção | 10% | | |
| Nível de risco | 5% | | |

Depois, recomendação por caso de uso (recomendação | justificativa | fornecedor
se comprar).

### 4. Critérios de avaliação
Requisitos obrigatórios (SOC 2, residência de dados, API, SSO, logs de auditoria)
e desejáveis.

### 5. Análise de custo
Cenário construir (desenvolvimento, infra, manutenção, treinamento) vs comprar
(licença, implementação, integração, treinamento), em 3 anos.

### 6. Shortlist de fornecedores
Primários recomendados (com justificativa, aderência X/10, custo estimado) e os
para avaliar (demo/POC).

### 7. Riscos e negociação
Tabela de riscos (fornecedor, lock-in, segurança, mitigação) e pontos de
alavancagem na negociação (descontos multi-ano, volume, bundling, cláusulas de
portabilidade e saída).

## Formato de saída
- Tabelas comparativas; nomes específicos de fornecedores.
- Estimativas de custo onde possível; recomendações claras e acionáveis.
```

## Saída esperada
Markdown com comparação de plataformas, matriz construir vs comprar por caso de
uso, análise de custo 3 anos e shortlist de fornecedores.
