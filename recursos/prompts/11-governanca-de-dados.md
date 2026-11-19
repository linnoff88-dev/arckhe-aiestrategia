# 11 — Framework de Governança de Dados

**Objetivo:** estruturar a governança de dados de `{empresa}` para sustentar
iniciativas de IA (papéis, classificação, qualidade, ciclo de vida, privacidade).

## Prompt (cole e use)

```
Contexto da empresa:
{empresa} — {contexto}

Pesquisa / insumos (use inventário, regulatório e política de IA, se gerados):
{pesquisa}

# Tarefa: Framework de Governança de Dados

Com base no inventário, no contexto regulatório e na política de IA acima, crie
um framework de governança de dados para iniciativas de IA, em markdown PT-BR.

## Seções obrigatórias

### 1. Resumo executivo
Maturidade de governança, riscos-chave, recomendações prioritárias, recursos.

### 2. Visão e princípios
Dado como ativo, qualidade na origem, segurança por design, transparência,
compliance em primeiro lugar.

### 3. Estrutura de governança
Modelo organizacional (Conselho → Escritório de governança → Stewards de domínio
e técnicos) e tabela de papéis & responsabilidades.

### 4. Classificação de dados
Níveis (Público/Interno/Confidencial/Restrito) com definição, exemplos e
requisitos de tratamento. Classificações específicas de IA (tipo de dado |
treinamento | input | output).

### 5. Qualidade de dados
Dimensões (acurácia, completude, consistência, atualidade, unicidade, validade)
com medição e meta. Monitoramento por sistema.

### 6. Ciclo de vida do dado
Estágios (criação, armazenamento, processamento, compartilhamento, arquivamento,
descarte) com controles e retenção. Ciclo de vida específico de IA (coleta,
preparação, treinamento, inferência, atualização de modelo).

### 7. Privacidade & proteção
Princípios (minimização, limitação de propósito, consentimento, direitos do
titular). Compliance (LGPD/GDPR e setor). Controles (anonimização,
pseudonimização, criptografia, controle de acesso).

### 8. Gestão de metadados
Padrões (técnico, de negócio, operacional) e requisitos do catálogo de dados.

### 9. Acesso & segurança
Modelo de controle de acesso por classificação e acesso de modelos de IA
(internos, ferramentas externas, modelos de fornecedor com DPA).

### 10. Roadmap de implementação
Fase 1 fundação (1-3 meses), Fase 2 construção (4-6 meses), Fase 3 escala
(7-12 meses).

### 11. Métricas & monitoramento
Tabela: métrica | meta | frequência | dono.

## Formato de saída
- Linguagem de governança profissional; políticas e procedimentos específicos.
- Customize ao setor; papéis claros; passos de implementação acionáveis.
```

## Saída esperada
Markdown com estrutura de governança, classificação, qualidade, ciclo de vida,
privacidade (LGPD), metadados, acesso e roadmap de implementação.
