# Arsenal — recursos reutilizáveis da Fábrica de Estratégia de IA

Arquivos prontos para copiar e usar. São o "arsenal" que você leva do curso:
skills do Claude Code, definições de subagentes, os 15 prompts de entregáveis,
templates comerciais e diagramas. Tudo em PT-BR, adaptado do repo
`ai-strategy-factory`.

Use isto para montar pacotes de consultoria de IA: pesquisar uma empresa,
diagnosticá-la, gerar os entregáveis e empacotar para o cliente.

## Mapa rápido

```
recursos/
├── README.md                      # este índice
├── skills/
│   ├── diagnostico-ia/SKILL.md    # diagnóstico: maturidade + quick wins + roadmap
│   └── gerar-entregavel/SKILL.md  # markdown → .docx / .pptx (e .xlsx / .pdf)
├── agentes/
│   ├── pesquisador-empresa.md     # subagente: pesquisa → CompanyContext
│   └── redator-estrategia.md      # subagente: pesquisa + framework → entregável
├── prompts/                       # 15 prompts de entregáveis (paste-ready)
│   ├── 01-inventario-tecnologico.md
│   ├── 02-dores-por-departamento.md
│   ├── 03-diagramas.md
│   ├── 04-maturidade.md
│   ├── 05-roadmap.md
│   ├── 06-quick-wins.md
│   ├── 07-comparacao-fornecedores.md
│   ├── 08-consolidacao-licencas.md
│   ├── 09-calculadora-roi.md
│   ├── 10-politica-de-ia.md
│   ├── 11-governanca-de-dados.md
│   ├── 12-gestao-da-mudanca.md
│   ├── 13-biblioteca-de-prompts.md
│   ├── 14-biblioteca-de-casos-de-uso.md
│   └── 15-glossario.md
├── templates/
│   ├── sow.md                     # declaração de trabalho (PT-BR)
│   ├── deck-executivo.md          # outline do deck slide a slide
│   ├── roadmap-30-60-90.md        # roadmap 30/60/90/180/360 em branco
│   └── roi-calculator.md          # estrutura da planilha de ROI (cores/fórmulas)
└── diagramas/
    ├── pipeline.mmd               # pipeline 3 fases (Pesquisa→Síntese→Geração)
    ├── estado-atual-vs-futuro.mmd # arquitetura atual vs futura (exemplo)
    └── README.md                  # como renderizar e usar
```

## O que é cada recurso (e a que módulo pertence)

### Skills (Claude Code)
Skills são capacidades reutilizáveis que disparam sozinhas pela `description`.
Copie a pasta da skill para `~/.claude/skills/` (global) ou `.claude/skills/`
(do projeto).

| Skill | O que faz | Módulo |
|---|---|---|
| `skills/diagnostico-ia/` | Recebe a descrição de uma empresa, aplica a escala de maturidade 1-5, lista quick wins e monta um roadmap 30/60/90. Saída em markdown. | T3 · M3.2 |
| `skills/gerar-entregavel/` | Converte um markdown de entregável em `.docx` e `.pptx` (e `.xlsx`/`.pdf`) com python-docx / python-pptx. | T3 · M3.3 |

### Agentes (subagentes)
Definições de subagentes — trabalho isolado, com contexto e ferramentas próprios.
Use como referência para criar o agente no Claude Code.

| Agente | O que faz | Módulo |
|---|---|---|
| `agentes/pesquisador-empresa.md` | Pesquisa a empresa na web (9 categorias) e devolve um `CompanyContext` estruturado com fontes. | T3 · M3.4 / T4 · M4.1 |
| `agentes/redator-estrategia.md` | Recebe a pesquisa + um prompt de entregável e rascunha o entregável em markdown. | T3 · M3.4 / T4 · M4.2 |

### Prompts (15 entregáveis)
Um arquivo por entregável, com objetivo, o **prompt pronto para colar** (com
placeholders `{empresa}` / `{contexto}` / `{pesquisa}`) e o formato de saída.
São a adaptação PT-BR dos 15 prompts do repo. Módulo: **T4 · M4.2**.

| # | Arquivo | Entregável |
|---|---|---|
| 01 | `01-inventario-tecnologico.md` | Inventário tecnológico & infraestrutura de dados |
| 02 | `02-dores-por-departamento.md` | Matriz de dores por departamento |
| 03 | `03-diagramas.md` | Diagramas Mermaid (estado atual + futuro) |
| 04 | `04-maturidade.md` | Maturidade & prontidão para IA (1-5) |
| 05 | `05-roadmap.md` | Roadmap 30/60/90/180/360 |
| 06 | `06-quick-wins.md` | Vitórias rápidas |
| 07 | `07-comparacao-fornecedores.md` | Comparação de fornecedores & construir vs comprar |
| 08 | `08-consolidacao-licencas.md` | Consolidação de licenças |
| 09 | `09-calculadora-roi.md` | Calculadora de ROI & custo |
| 10 | `10-politica-de-ia.md` | Política de uso aceitável de IA |
| 11 | `11-governanca-de-dados.md` | Governança de dados |
| 12 | `12-gestao-da-mudanca.md` | Gestão da mudança & treinamento |
| 13 | `13-biblioteca-de-prompts.md` | Biblioteca de prompts |
| 14 | `14-biblioteca-de-casos-de-uso.md` | Biblioteca de casos de uso |
| 15 | `15-glossario.md` | Glossário de termos de IA |

### Templates (comercial)
Documentos de venda e entrega, em branco para preencher. Módulo: **T5 · M5.3**
(e M5.2 para preço).

| Template | O que é |
|---|---|
| `templates/sow.md` | Declaração de Trabalho: escopo, entregáveis, prazo, preço, premissas, exclusões. |
| `templates/deck-executivo.md` | Outline do deck que fecha (problema → diagnóstico → quick wins → roadmap → ROI → governança → próximos passos). |
| `templates/roadmap-30-60-90.md` | Roadmap 30/60/90/180/360 em branco. |
| `templates/roi-calculator.md` | Estrutura da planilha de ROI: abas, fórmulas e convenção de cores. |

### Diagramas
Mermaid + guia de renderização. Módulo: **T4 · M4.3**.

| Arquivo | O que é |
|---|---|
| `diagramas/pipeline.mmd` | O pipeline de 3 fases da Fábrica. |
| `diagramas/estado-atual-vs-futuro.mmd` | Arquitetura atual vs futura (exemplo a adaptar). |
| `diagramas/README.md` | Como renderizar (eraser.io, mermaid.live, `beautiful-mermaid`) e usar nos entregáveis. |

## Como usar (fluxo do pacote)

1. **Pesquisar** — rode o agente `pesquisador-empresa` → recebe um `CompanyContext`.
2. **Diagnosticar** — rode a skill `diagnostico-ia` com esse contexto → maturidade
   + quick wins + roadmap 30/60/90.
3. **Gerar entregáveis** — para cada peça, use o prompt de `prompts/` (preenchendo
   `{empresa}/{contexto}/{pesquisa}`); o agente `redator-estrategia` rascunha o
   markdown.
4. **Diagramar** — gere o Mermaid com `03-diagramas.md`, renderize (ver
   `diagramas/README.md`) e insira nos documentos.
5. **Empacotar** — converta os markdowns em `.docx`/`.pptx` com a skill
   `gerar-entregavel`; monte o ROI em `.xlsx` pelo `roi-calculator.md`.
6. **Vender** — preencha o `deck-executivo.md` e o `sow.md` para a reunião.

Saída padrão dos artefatos: `~/projetos/output/<empresa>/`.

## Fidelidade

Tudo aqui é adaptação PT-BR (traduzida e enxuta) do repo `ai-strategy-factory`:
os 15 prompts de `synthesis/prompts/`, os modelos de `models.py`, as 9 categorias
de `research/query_templates.py`, a geração de documentos de
`.claude/document-creation-skills.md` e a arquitetura de `docs/ARCHITECTURE.md`.
Não inventa APIs — espelha o que o repo faz.
