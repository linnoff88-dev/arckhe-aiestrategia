# 01 — Inventário Tecnológico & Infraestrutura de Dados

**Objetivo:** mapear o cenário tecnológico atual de `{empresa}` e avaliar o
quanto ela está pronta para IA (dados, integrações, infraestrutura).

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa:
{pesquisa}

# Tarefa: Inventário Tecnológico & Avaliaçêo de Infraestrutura de Dados

Com base no contexto e na pesquisa acima, crie um inventário tecnológico
completo de {empresa}, em markdown PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
- Visêo geral do cenário tecnológico atual
- Principais achados e lacunas críticas
- Prontidêo para adoçêo de IA (avaliaçêo de alto nível)

### 2. Stack tecnológico atual
Tabela com as colunas:
| Categoria | Ferramenta/Plataforma | Funçêo | Pronta p/ IA | Integraçêo de dados |

Categorias: sistemas centrais (ERP, CRM), comunicaçêo & colaboraçêo, dados &
analytics, desenvolvimento & DevOps, segurança & compliance, ferramentas do
setor.

### 3. Avaliaçêo da infraestrutura de dados
- Fontes de dados (bancos internos, integrações de terceiros, entrada manual,
  feeds externos)
- Indicadores de qualidade (estruturado vs nêo-estruturado, atualidade,
  problemas conhecidos, maturidade de governança)
- Acessibilidade (APIs, exportaçêo, tempo real, restrições de segurança/privacidade)

### 4. Cenário de integrações
Descreva como os sistemas se conectam: integrações principais, direçêo do fluxo
de dados, métodos (API, transferência de arquivo, manual) e lacunas.

### 5. Prontidêo para IA
| Dimensêo | Estado atual | Lacuna | Prioridade |
|---|---|---|---|
| Qualidade dos dados | | | |
| Acessibilidade dos dados | | | |
| Infraestrutura de computaçêo | | | |
| Skills técnicos | | | |
| Capacidade de integraçêo | | | |

### 6. Recomendações
- Ações imediatas (0-30 dias)
- Prioridades de curto prazo (30-90 dias)
- Considerações de longo prazo (90+ dias)

## Formato de saída
- Markdown, com as tabelas indicadas.
- Específico com nomes de ferramentas onde houver.
- Marque suposições claramente onde a informaçêo for limitada.
- Recomendações acionáveis e priorizadas.
```

## Saída esperada
Documento markdown com resumo executivo, tabela de stack, avaliaçêo de dados,
mapa de integrações, tabela de prontidêo para IA e recomendações priorizadas.
