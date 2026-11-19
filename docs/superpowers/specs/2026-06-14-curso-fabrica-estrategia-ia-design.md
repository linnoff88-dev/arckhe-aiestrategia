# Curso: Fábrica de Estratégia de IA — Vire Consultor de IA

> **Spec / Blueprint** — fonte única de verdade para o build.
> **Data:** 2026-06-14 · **Formato:** INEMA.CLUB (skill `formato-curso`) · **Idioma:** PT-BR
> **Repo:** `inematds/aiestrategia` → `https://inematds.github.io/aiestrategia/` · **Portal:** inema.club

---

## 1. Resumo executivo

Curso prático, mão na massa, para quem quer **entrar na área de IA e de consultoria de IA**. O aluno **constrói a própria Fábrica de Estratégia de IA** (uma ferramenta que gera pacotes de consultoria — 19 entregáveis — automaticamente, com Claude Code + Perplexity + Gemini) e, no mesmo movimento, aprende a **se posicionar e vender como consultor**. Cada habilidade técnica é enquadrada como uma capacidade vendável.

**Promessa:** sair do zero e terminar com (1) uma fábrica funcionando, (2) um arsenal de skills/agentes/prompts reutilizáveis, e (3) um primeiro entregável de consultoria pronto para apresentar a um cliente real.

**Tese central (do material-fonte):** *entrada mínima, saída máxima*. Duas caixas de texto → pacote de consultoria impecável. Custo < US$1, valor de mercado de milhares.

## 2. Público & objetivos

- **Público:** iniciante a intermediário, **não exige ser dev**. Orquestra tudo via Claude Code.
- **Objetivo de aprendizagem:** rápido mas completo — do conceito ao entregável vendável.
- **Resultado final (capstone):** rodar a Fábrica para uma empresa real e montar a apresentação + SOW.

## 3. Ângulo & decisões

- **Ângulo C (híbrido):** espinha = construir a Fábrica (as 5 fases do material-fonte `IA-metodologia.txt`); camada de negócio enquadra cada habilidade como serviço de consultoria; fecha com trilha de entrega/venda + capstone.
- **Fonte de conteúdo:** repo `ai-strategy-factory` (código real, 15 prompts, TLDRs BCG/KPMG/McKinsey) + `IA-metodologia.txt` (método das 5 fases) + pesquisa de mercado.
- **Fidelidade:** referenciar sempre o repo do usuário (`inematds/ai-strategy-factory`), não o upstream.

## 4. Mecânica pedagógica

### 4.1 Sistema de níveis (subir de nível)
Cada trilha é um **nível** com badge. O index (landing) mostra a progressão.

| Nível | Badge | Trilha | Cor |
|---|---|---|---|
| 1. Aprendiz | 🥉 | Fundamentos & Setup | Emerald (T1) |
| 2. Sintetizador | 🥈 | Síntese de Conhecimento | Blue (T2) |
| 3. Construtor | 🥇 | Skills & Agentes | Purple (T3) |
| 4. Engenheiro | 💎 | A Fábrica | Amber (T4) |
| 5. Consultor | 👑 | Da Fábrica ao Cliente | Teal (T5) |

### 4.2 Missões (exercícios)
Cada módulo termina com uma **Missão**: tarefa curta com **vitória concreta** e um **artefato que o aluno leva**. Padrão de copy: "Ao fim você tem **X funcionando** e pode **cobrar Y por isso**." Sem coachzinho (regra de tom INEMA): motivação vem do **payoff concreto** e da **progressão de nível**, não de exclamação.

- Cada Missão: objetivo (1 frase) → passos (3-5) → critério de sucesso verificável → "o que você ganhou".
- **Desafio relâmpago** opcional por trilha (mais difícil, marca de maestria).

### 4.3 Recursos reutilizáveis (entregáveis do curso)
Pasta `recursos/` no repo, com skills, agentes, prompts e templates prontos para copiar e usar (detalhe na §6). É o cumprimento do pedido "exemplos práticos facilmente utilizáveis, criando skills, agentes e outros recursos".

### 4.4 Diagramas
- **Dentro das páginas:** cada módulo de conteúdo tem ≥1 **SVG futurista inline** (regra `formato-curso` #17) na cor da trilha + ciano.
- **Como conteúdo ensinado:** Mermaid (estado atual vs futuro), com `recursos/diagramas/` e ponteiros para **eraser.io** e a skill `beautiful-mermaid`.

### 4.5 Tom de voz (INEMA)
Direto, brasileiro ("você"), concreto (números, R$, %), sóbrio. Parágrafos de 3-4 linhas. Sem floreio, sem "vamos juntos".

## 5. Estrutura completa (5 trilhas · 16 módulos · 6 tópicos cada)

> Cada módulo: página `modulo-X-Y.html` (500-800 linhas, 6-8 seções, ≥1 SVG, variedade de componentes) **e** entrada no index da trilha (accordion de 6 tópicos × 3 seções "O que é / Por que aprender / Conceitos-chave"). Cada módulo fecha com uma **Missão**.

### T1 — Fundamentos & Setup (Emerald) · Nível Aprendiz · 3 módulos
**M1.1 — A oportunidade: IA + consultoria agora**
1. Por que 2026 é o momento (dados de mercado — usar pesquisa)
2. O que é estratégia/consultoria de IA na prática
3. A tese "entrada mínima, saída máxima"
4. Da ferramenta à renda (uso pessoal / na empresa / cliente pago)
5. O mito do "preciso ser programador"
6. Como o curso funciona (níveis, missões, recursos)
*Missão:* escrever sua "tese de consultor" em 3 frases (nicho + dor + oferta).

**M1.2 — Anatomia da Fábrica**
1. Os 19 entregáveis (panorama)
2. O pipeline de 3 fases (Pesquisa → Síntese → Geração)
3. O que cada fase faz e por quê
4. Por que o output parece consultoria de elite (BCG/KPMG)
5. Demonstração: um pacote real, peça por peça
6. O mapa do curso (o que você vai construir até o capstone)
*Missão:* listar, para uma empresa que você conhece, 3 entregáveis que mais venderiam.

**M1.3 — Montando o arsenal (setup)**
1. Claude Code: seu copiloto de construção
2. Conta + chave Perplexity (pesquisa ao vivo)
3. Conta + chave Gemini (síntese barata, contexto gigante)
4. Clonar e rodar o repo (`inematds/ai-strategy-factory`)
5. Build in public: a mentalidade (mostrar a bagunça, não só o resultado)
6. Gestão de custo: quick vs deep, ~US$1, dividir pedidos
*Missão:* rodar a Fábrica em modo quick para 1 empresa e abrir os arquivos.

### T2 — Síntese de Conhecimento (Blue) · Nível Sintetizador · 3 módulos
**M2.1 — Os frameworks que valem ouro** (fonte: TLDRs + prompts reais)
1. AI Maturity Assessment (escala 1-5, readiness)
2. Quick Wins (matriz esforço × impacto)
3. Build vs Buy (decisão de fornecedor)
4. ROI de IA (custo-benefício, projeções)
5. Roadmap 30/60/90/180/360 dias
6. Governança de dados & política de uso aceitável
*Missão:* aplicar Quick Wins a um setor e listar 3 vitórias rápidas.

**M2.2 — RAG preguiçoso: PDF gigante → cheat sheet** (fonte: `pdf_to_cheatsheet.py`, Fase 1)
1. O problema do contexto (PDFs de 28-46 páginas estouram o limite)
2. Chunking em blocos de ~10k tokens
3. O prompt de síntese (extrair só o valioso; cortar buzzword)
4. Gemini 2.5 Flash: barato e com contexto gigante
5. Montar o cheat sheet ultra-comprimido
6. `pdf_to_cheatsheet.py` na prática
*Missão:* transformar 1 PDF de consultoria num cheat sheet de 1 página.

**M2.3 — Seu cérebro de consultor (base de conhecimento)**
1. Por que destilar conhecimento (token é barato, contexto é caro)
2. Curar fontes (McKinsey, BCG, KPMG, OpenAI, IBM)
3. Anatomia de um cheat sheet reutilizável
4. Versionar e organizar a base
5. Injetar contexto sem estourar tokens (RAG preguiçoso aplicado)
6. Sua biblioteca pessoal de consultor
*Missão:* montar uma pasta `conhecimento/` com 3 cheat sheets curados.

### T3 — Skills & Agentes (Purple) · Nível Construtor · 4 módulos
**M3.1 — Skills e subagentes: o que são e quando usar**
1. O que é uma skill (capacidade reutilizável, sob demanda)
2. O que é um subagente (trabalho isolado, contexto próprio)
3. Skill vs agente: quando cada um
4. Anatomia de uma skill (`SKILL.md`, frontmatter `name`/`description`)
5. Onde skills e agentes vivem no Claude Code
6. O ecossistema de recursos reutilizáveis (por que isso vira ativo)
*Missão:* mapear 3 tarefas suas que viram skill e 2 que viram agente.

**M3.2 — Construa sua primeira skill (`diagnostico-ia`)**
1. Definir o gatilho (a `description` que faz a skill disparar)
2. Escrever o corpo (passos claros, determinísticos)
3. Anexar referências (os cheat sheets da T2)
4. Testar a skill com um caso real
5. Iterar e empacotar
6. Versionar e compartilhar
*Missão:* skill `diagnostico-ia` rodando e cuspindo um mini-diagnóstico.

**M3.3 — A skill de documentos (DocX/PPTX/Excel/PDF)** (fonte: `document-creation-skills.md`, Fase 2)
1. Por que gerar documentos programaticamente
2. `python-docx` — relatórios Word
3. `python-pptx` — apresentações (RGBColor, layouts)
4. `openpyxl` — Excel com fórmulas e convenção de cores
5. `reportlab` — PDF (Platypus)
6. Empacotar como skill `gerar-entregavel`
*Missão:* gerar 1 `.docx` + 1 `.pptx` a partir de um markdown.

**M3.4 — Construa seu subagente (pesquisador & redator)**
1. Anatomia de um subagente (system prompt, ferramentas, saída)
2. O agente `pesquisador-empresa` (coleta contexto estruturado)
3. O agente `redator-estrategia` (rascunha entregável a partir de pesquisa + framework)
4. Saída estruturada (schema, JSON confiável)
5. Orquestrar skill + agentes juntos
6. Quando paralelizar agentes
*Missão:* agente `pesquisador-empresa` retornando um `CompanyContext` preenchido.

### T4 — A Fábrica (Amber) · Nível Engenheiro · 3 módulos
**M4.1 — Pesquisa ao vivo com Perplexity** (fonte: `query_templates.py`, Fase 3)
1. Por que pesquisa ao vivo (não ficar estático/desatualizado)
2. Quick vs Deep (sonar / sonar-pro / deep-research) e custo
3. Contexto temporal (injetar a data atual nas queries)
4. As 9 categorias de query (empresa, setor, concorrência, tech, IA, dores, regulatório, liderança, notícias)
5. Agregar e tratar resultados (degradação graciosa)
6. Montar o `ResearchOutput`
*Missão:* pesquisa quick estruturada de 1 empresa, 9 categorias.

**M4.2 — Os 15 prompts de entregáveis** (fonte: `synthesis/prompts/*.py`)
1. Anatomia de um prompt de entregável profissional
2. Avaliação (tech inventory, pain points, maturity)
3. Planejamento (roadmap, quick wins, ROI)
4. Implementação (build vs buy, licenças, casos de uso)
5. Governança (política de IA, dados, gestão de mudança)
6. Recursos (biblioteca de prompts, glossário) + adaptar ao PT-BR
*Missão:* adaptar 1 prompt de entregável e gerar o markdown.

**M4.3 — Orquestração, retomada e diagramas que vendem** (fonte: ARCHITECTURE.md, `mermaid_diagrams.py`)
1. O orquestrador de pipeline (cada etapa confirma antes de seguir)
2. Checkpoints e `state.json` (progress tracking)
3. Retomar sessão quando o contexto enche
4. Mermaid: estado atual vs futuro
5. Renderizar Mermaid → PNG (e usar eraser.io / `beautiful-mermaid`)
6. Empacotar o pacote completo para download
*Missão:* rodar a Fábrica ponta a ponta e gerar os diagramas.

### T5 — Da Fábrica ao Cliente (Teal) · Nível Consultor · 3 módulos
**M5.1 — Frontend e empacotamento** (fonte: Fase 5, webapp)
1. A interface mínima (nome + descrição + profundidade + enviar)
2. Rodar a webapp local (localhost:8888)
3. Progresso em tempo real (SSE) e download dos assets
4. Organizar o pacote por pastas
5. Marca: deixar o entregável com a sua cara
6. Hospedar/entregar o pacote
*Missão:* gerar e empacotar um pacote com a sua identidade.

**M5.2 — Posicionamento, oferta e preço** (fonte: pesquisa de mercado)
1. Achar seu nicho (setor + dor específica)
2. A oferta produtizada (diagnóstico de IA como produto)
3. Precificação (custo < US$1 vs valor de mercado; faixas reais)
4. Formatos: projeto, retainer, produtizado
5. Conseguir os primeiros clientes (canais, prova)
6. Ética e expectativa (o que a Fábrica é e não é)
*Missão:* escrever sua oferta de 1 página (nicho, entregável, preço).

**M5.3 — A apresentação que fecha + Capstone**
1. O deck executivo (estrutura que decide)
2. O SOW / declaração de trabalho (escopo, preço, prazo)
3. Conduzir a reunião (do diagnóstico ao próximo passo)
4. Objeções comuns e respostas
5. **Capstone:** Fábrica rodando para um cliente real
6. Próximos passos (evoluir a fábrica, novos entregáveis)
*Missão (capstone):* pacote completo + deck + SOW de uma empresa real.

## 6. Recursos reutilizáveis (`recursos/`)

Arquivos reais, prontos para copiar. Adaptados do repo (PT-BR), curados.

```
recursos/
├── README.md                      # índice + como usar cada recurso
├── skills/
│   ├── diagnostico-ia/SKILL.md    # diagnóstico (maturity+quick wins+roadmap) de empresa descrita
│   └── gerar-entregavel/SKILL.md  # markdown → .docx/.pptx (wrap document-creation)
├── agentes/
│   ├── pesquisador-empresa.md     # subagente: pesquisa → CompanyContext estruturado
│   └── redator-estrategia.md      # subagente: pesquisa + framework → entregável
├── prompts/                       # 15 prompts de entregáveis em PT-BR (paste-ready)
│   ├── 01-tech-inventory.md ... 15-glossario.md
├── templates/
│   ├── sow.md                     # statement of work PT-BR
│   ├── deck-executivo.md          # outline do deck
│   ├── roadmap-30-60-90.md
│   └── roi-calculator.md          # estrutura da planilha (convenção de cores)
└── diagramas/
    ├── pipeline.mmd               # Mermaid do pipeline 3 fases
    ├── estado-atual-vs-futuro.mmd
    └── README.md                  # eraser.io + beautiful-mermaid
```

## 7. Identidade visual

- **Emoji do curso:** 🏭
- **Nome:** "Fábrica de Estratégia de IA — Vire Consultor de IA"
- **Cores por trilha:** T1 Emerald, T2 Blue, T3 Purple, T4 Amber, T5 Teal (sequência cromática INEMA).
- **Estética:** dark premium, Tailwind via CDN, Inter, SVG inline futurista, light mode obrigatório. Zero imagens raster nas páginas (PNG opcional via inemaimg só como extra decorativo — não substitui SVG).

## 8. Plano de publicação

1. **Git:** `git init` em `/home/nmaldaner/projetos/aiestrategia`, `.gitignore` (ignora `_reference/`, `docs/fontes/`, `venv`), commits incrementais.
2. **Repo remoto:** criar `inematds/aiestrategia` (público) via `gh`, push `main`.
3. **GitHub Pages:** habilitar Pages na branch `main` (root). Adicionar `.nojekyll`. URL `https://inematds.github.io/aiestrategia/`.
4. **Portal inema.club** (`/home/nmaldaner/projetos/portal`):
   - `src/data/courses.ts` → `platformsData` (ordem alfabética, id = max+1): title "Fábrica de Estratégia de IA — Vire Consultor de IA", icon 🏭, tags ['IA','Consultoria','Claude Code','Estratégia'], url Pages.
   - `updatesData` (topo): `{ date:'2026-06-14', title:'…', type:'novo', url:… }`.
   - Trilha hardcoded em `Portal.tsx`/`PortalV2.tsx`: só se encaixar numa trilha existente; senão, standalone.
   - Commit + push (Vercel faz deploy).

## 9. Checklist de build & conformidade `formato-curso`

Por página (ver `CHECKLIST_REVISAO.md` + 17 erros críticos):
- [ ] Nav completo idêntico em TODAS as páginas (logo + INEMA.CLUB sky-400 + 5 botões de trilha + theme toggle); trilha ativa destacada.
- [ ] Light mode CSS completo (4 partes + cor de acento da trilha + bordas dark suavizadas).
- [ ] Botões `justify-start`; tópicos com número em círculo; título de módulo `text-2xl`.
- [ ] Index de trilha: header + stats(4) + **Mapa da trilha** + "Conteudo detalhado" + cards de módulo (cada um com 6-8 tópicos accordion de 3 seções + "Ver em Modal" iframe + "Ver Completo").
- [ ] Módulo: breadcrumb + header stats(4) + 6-8 seções variadas (≥2 grids ✓/✗, ≥1 timeline, ≥2 tip boxes, code box quando útil) + ≥1 SVG futurista + Resumo final + Missão.
- [ ] Hero SVG no index de cada trilha.
- [ ] Tom INEMA; missões com payoff concreto.

**Ordem de build:** (a) scaffold + git; (b) golden reference: `index.html` + `curso/index.html` + `curso/trilha1/index.html` + `curso/trilha1/modulo-1-1.html`; (c) fan-out por trilha (subagentes seguindo golden + este spec); (d) `recursos/`; (e) auditoria `revisar-curso` + fix; (f) publicação.

## 10. Fontes

- Repo: `_reference/ai-strategy-factory/` (README, ARCHITECTURE.md, CLAUDE.md, `synthesis/prompts/*.py`, `research/query_templates.py`, `generation/*`, `Consulting Guides TLDR/*`, `.claude/document-creation-skills.md`).
- Método: `docs/fontes/IA-metodologia.txt` (5 fases).
- Pesquisa de mercado: agente web (em curso) — dados/estatísticas para ganchos motivacionais e a trilha T5.
- Template: skill `formato-curso` (`MASTER_COMPLETO.md`, `SVG-FUTURISTA.md`, `DESIGN-SYSTEM.md`, `CHECKLIST_REVISAO.md`).
