# 01 — Inventário Tecnológico & Infraestrutura de Dados

**Objetivo:** mapear o cenário tecnológico atual de `{empresa}` e avaliar o
quanto ela está pronta para IA (dados, integrações, infraestrutura).

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa:
{pesquisa}

# Tarefa: Inventário Tecnológico & Avaliação de Infraestrutura de Dados

Com base no contexto e na pesquisa acima, crie um inventário tecnológico
completo de {empresa}, em markdown PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
- Visão geral do cenário tecnológico atual
- Principais achados e lacunas críticas
- Prontidão para adoção de IA (avaliação de alto nível)

### 2. Stack tecnológico atual
Tabela com as colunas:
| Categoria | Ferramenta/Plataforma | Função | Pronta p/ IA | Integração de dados |

Categorias: sistemas centrais (ERP, CRM), comunicação & colaboração, dados &
analytics, desenvolvimento & DevOps, segurança & compliance, ferramentas do
setor.

### 3. Avaliação da infraestrutura de dados
- Fontes de dados (bancos internos, integrações de terceiros, entrada manual,
  feeds externos)
- Indicadores de qualidade (estruturado vs não-estruturado, atualidade,
  problemas conhecidos, maturidade de governança)
- Acessibilidade (APIs, exportação, tempo real, restrições de segurança/privacidade)

### 4. Cenário de integrações
Descreva como os sistemas se conectam: integrações principais, direção do fluxo
de dados, métodos (API, transferência de arquivo, manual) e lacunas.

### 5. Prontidão para IA
| Dimensão | Estado atual | Lacuna | Prioridade |
|---|---|---|---|
| Qualidade dos dados | | | |
| Acessibilidade dos dados | | | |
| Infraestrutura de computação | | | |
| Skills técnicos | | | |
| Capacidade de integração | | | |

### 6. Recomendações
- Ações imediatas (0-30 dias)
- Prioridades de curto prazo (30-90 dias)
- Considerações de longo prazo (90+ dias)

## Formato de saída
- Markdown, com as tabelas indicadas.
- Específico com nomes de ferramentas onde houver.
- Marque suposições claramente onde a informação for limitada.
- Recomendações acionáveis e priorizadas.
```

## Saída esperada
Documento markdown com resumo executivo, tabela de stack, avaliação de dados,
mapa de integrações, tabela de prontidão para IA e recomendações priorizadas.
