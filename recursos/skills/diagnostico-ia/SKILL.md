---
name: diagnostico-ia
description: >-
  Use quando o usuário pedir um diagnóstico de IA de uma empresa — avaliar o
  nível de maturidade em IA, achar quick wins (vitórias rápidas) e montar um
  mini-roadmap 30/60/90 a partir de uma descrição da empresa (nome, setor,
  porte, dores, stack). Acione com pedidos como "faz um diagnóstico de IA da
  empresa X", "avalia a maturidade de IA dessa empresa", "onde essa empresa
  está em IA e por onde começar", "monta um diagnóstico pra eu apresentar a um
  cliente". É a primeira peça vendável da Fábrica de Estratégia de IA.
---

# Diagnóstico de IA (maturidade + quick wins + mini-roadmap)

Produz um diagnóstico curto e vendável de uma empresa: onde ela está em IA
(escala 1-5), 3-5 vitórias rápidas, e um plano 30/60/90 dias. Saída em markdown
pronto para virar slide ou .docx (ver skill `gerar-entregavel`).

Este é um diagnóstico **rápido** (modo quick): roda só com a descrição que o
usuário deu, sem precisar de pesquisa ao vivo. Se houver pesquisa estruturada
disponível (um `CompanyContext` do agente `pesquisador-empresa`), use-a para
embasar as notas. Sem pesquisa, marque suposições com `(suposição)`.

## Referências a anexar

Antes de gerar, leia/anexe os cheat sheets de frameworks da base de
conhecimento do curso (pasta `conhecimento/` montada na T2), em especial:

- **AI Maturity** — a escala 1-5 (Passivo → Transformacional), baseada na curva
  de maturidade da BCG.
- **Quick Wins** — matriz esforço × impacto e critérios de seleção.
- **Roadmap 30/60/90** — fases e marcos.

Se a pasta `conhecimento/` não existir, use as escalas embutidas abaixo (são o
resumo fiel desses frameworks).

## Passos (determinísticos)

### 1. Coletar o contexto da empresa

Extraia da descrição do usuário (ou do `CompanyContext`):

- `nome` da empresa
- `setor` / indústria
- `porte` (nº de funcionários → pequena <100, média 100-500, grande 500-2000,
  enterprise 2000+)
- `localização`
- `stack` tecnológico conhecido (ERP, CRM, ferramentas, nuvem)
- `objetivos` declarados
- `dores` / desafios

Falta de dado **não** bloqueia. Liste o que falta em "Suposições e lacunas".

### 2. Aplicar a escala de Maturidade de IA (1-5)

Posicione a empresa em **um** dos 5 estágios e justifique com evidência da
descrição:

| Nível | Estágio | Sinais |
|---|---|---|
| 1 | **Passivo** | Nenhuma iniciativa de IA, processos tradicionais/manuais |
| 2 | **Consciente** | Explorando IA, pilotos iniciais, uso pontual de ferramentas |
| 3 | **Ativo** | Vários projetos de IA, alguns em produção |
| 4 | **Operacional** | IA integrada a processos centrais |
| 5 | **Transformacional** | Organização nativa de IA, vantagem competitiva |

Depois, dê uma nota **1-5 por dimensão** numa tabela:

| Dimensão | Nota (1-5) | Evidência | Lacuna |
|---|---|---|---|
| Estratégia & Visão | | | |
| Dados & Infraestrutura | | | |
| Tecnologia & Ferramentas | | | |
| Talento & Skills | | | |
| Governança & Ética | | | |
| Cultura & Mudança | | | |
| Casos de uso & Valor | | | |

A nota geral do diagnóstico = estágio (1-5) + média das dimensões como reforço.

### 3. Identificar Quick Wins (vitórias rápidas)

Selecione 3-5 iniciativas que cabem nos critérios:

- Implementação em **< 60 dias**
- Investimento **baixo** (ferramentas SaaS ou recursos internos)
- Risco **baixo**
- ROI **demonstrável**
- Pré-requisitos **mínimos**

Classifique cada uma na matriz esforço × impacto e priorize as de **alto
impacto / baixo esforço**. Formato:

| # | Quick Win | Depto | Esforço | Impacto | Como (1 frase) |
|---|---|---|---|---|---|

### 4. Montar o mini-roadmap 30/60/90

Três fases, com objetivo e 2-4 ações por fase:

- **30 dias — Fundação:** governança mínima, auditoria de dados, priorizar quick
  wins, montar comitê/responsável.
- **60 dias — Vitórias rápidas:** lançar 2-3 quick wins, capturar as primeiras
  métricas de ROI, treinar usuários.
- **90 dias — Escala:** expandir os pilotos que deram certo, framework de
  medição, começar a Central de Excelência.

(Se o cliente pedir, estenda para 180/360 usando o template
`templates/roadmap-30-60-90.md`.)

### 5. Gerar a saída em markdown

Monte um único arquivo markdown com esta estrutura exata:

```markdown
# Diagnóstico de IA — {nome}

## Resumo executivo
- Nível de maturidade: {estágio} ({n}/5)
- 3-5 vitórias rápidas priorizadas
- Próximo passo recomendado

## Contexto da empresa
{setor, porte, localização, stack, objetivos, dores}

## Maturidade de IA
{estágio + parágrafo de evidência}
{tabela das 7 dimensões}

## Quick Wins
{tabela priorizada + 1 parágrafo por win do top 3}

## Roadmap 30/60/90
{3 fases com ações}

## Suposições e lacunas
{o que foi suposto; que dados pediríamos ao cliente}
```

Tom: direto, brasileiro ("você" / impessoal), concreto (números, R$, %), sóbrio.
Sem floreio. Toda nota precisa de evidência ou da marca `(suposição)`.

## Critério de sucesso

O arquivo abre como um diagnóstico que dá para apresentar a um cliente: posiciona
a empresa (1-5), entrega 3-5 quick wins acionáveis e um plano 30/60/90 — sem
inventar fatos não embasados.
