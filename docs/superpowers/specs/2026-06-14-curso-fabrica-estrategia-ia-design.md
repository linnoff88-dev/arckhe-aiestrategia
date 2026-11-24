# Curso: FÃ¡brica de EstratÃ©gia de IA â€” Vire Consultor de IA

> **Spec / Blueprint** â€” fonte Ãºnica de verdade para o build.
> **Data:** 2026-06-14 Â· **Formato:** ARCKHÉ AI (skill `formato-curso`) Â· **Idioma:** PT-BR
> **Repo:** `linnoff88-dev/aiestrategia` â†’ `https://linnoff88-dev.github.io/ Â· **Portal:** ARCKHÉ AI

---

## 1. Resumo executivo

Curso prÃ¡tico, mÃ£o na massa, para quem quer **entrar na Ã¡rea de IA e de consultoria de IA**. O aluno **constrÃ³i a prÃ³pria FÃ¡brica de EstratÃ©gia de IA** (uma ferramenta que gera pacotes de consultoria â€” 19 entregÃ¡veis â€” automaticamente, com Claude Code + Perplexity + Gemini) e, no mesmo movimento, aprende a **se posicionar e vender como consultor**. Cada habilidade tÃ©cnica Ã© enquadrada como uma capacidade vendÃ¡vel.

**Promessa:** sair do zero e terminar com (1) uma fÃ¡brica funcionando, (2) um arsenal de skills/agentes/prompts reutilizÃ¡veis, e (3) um primeiro entregÃ¡vel de consultoria pronto para apresentar a um cliente real.

**Tese central (do material-fonte):** *entrada mÃ­nima, saÃ­da mÃ¡xima*. Duas caixas de texto â†’ pacote de consultoria impecÃ¡vel. Custo < US$1, valor de mercado de milhares.

## 2. PÃºblico & objetivos

- **PÃºblico:** iniciante a intermediÃ¡rio, **nÃ£o exige ser dev**. Orquestra tudo via Claude Code.
- **Objetivo de aprendizagem:** rÃ¡pido mas completo â€” do conceito ao entregÃ¡vel vendÃ¡vel.
- **Resultado final (capstone):** rodar a FÃ¡brica para uma empresa real e montar a apresentaÃ§Ã£o + SOW.

## 3. Ã‚ngulo & decisÃµes

- **Ã‚ngulo C (hÃ­brido):** espinha = construir a FÃ¡brica (as 5 fases do material-fonte `IA-metodologia.txt`); camada de negÃ³cio enquadra cada habilidade como serviÃ§o de consultoria; fecha com trilha de entrega/venda + capstone.
- **Fonte de conteÃºdo:** repo `ai-strategy-factory` (cÃ³digo real, 15 prompts, TLDRs BCG/KPMG/McKinsey) + `IA-metodologia.txt` (mÃ©todo das 5 fases) + pesquisa de mercado.
- **Fidelidade:** referenciar sempre o repo do usuÃ¡rio (`linnoff88-dev/ai-strategy-factory`), nÃ£o o upstream.

## 4. MecÃ¢nica pedagÃ³gica

### 4.1 Sistema de nÃ­veis (subir de nÃ­vel)
Cada trilha Ã© um **nÃ­vel** com badge. O index (landing) mostra a progressÃ£o.

| NÃ­vel | Badge | Trilha | Cor |
|---|---|---|---|
| 1. Aprendiz | ðŸ¥‰ | Fundamentos & Setup | Emerald (T1) |
| 2. Sintetizador | ðŸ¥ˆ | SÃ­ntese de Conhecimento | Blue (T2) |
| 3. Construtor | ðŸ¥‡ | Skills & Agentes | Purple (T3) |
| 4. Engenheiro | ðŸ’Ž | A FÃ¡brica | Amber (T4) |
| 5. Consultor | ðŸ‘‘ | Da FÃ¡brica ao Cliente | Teal (T5) |

### 4.2 MissÃµes (exercÃ­cios)
Cada mÃ³dulo termina com uma **MissÃ£o**: tarefa curta com **vitÃ³ria concreta** e um **artefato que o aluno leva**. PadrÃ£o de copy: "Ao fim vocÃª tem **X funcionando** e pode **cobrar Y por isso**." Sem coachzinho (regra de tom ARCKHÉ): motivaÃ§Ã£o vem do **payoff concreto** e da **progressÃ£o de nÃ­vel**, nÃ£o de exclamaÃ§Ã£o.

- Cada MissÃ£o: objetivo (1 frase) â†’ passos (3-5) â†’ critÃ©rio de sucesso verificÃ¡vel â†’ "o que vocÃª ganhou".
- **Desafio relÃ¢mpago** opcional por trilha (mais difÃ­cil, marca de maestria).

### 4.3 Recursos reutilizÃ¡veis (entregÃ¡veis do curso)
Pasta `recursos/` no repo, com skills, agentes, prompts e templates prontos para copiar e usar (detalhe na Â§6). Ã‰ o cumprimento do pedido "exemplos prÃ¡ticos facilmente utilizÃ¡veis, criando skills, agentes e outros recursos".

### 4.4 Diagramas
- **Dentro das pÃ¡ginas:** cada mÃ³dulo de conteÃºdo tem â‰¥1 **SVG futurista inline** (regra `formato-curso` #17) na cor da trilha + ciano.
- **Como conteÃºdo ensinado:** Mermaid (estado atual vs futuro), com `recursos/diagramas/` e ponteiros para **eraser.io** e a skill `beautiful-mermaid`.

### 4.5 Tom de voz (ARCKHÉ)
Direto, brasileiro ("vocÃª"), concreto (nÃºmeros, R$, %), sÃ³brio. ParÃ¡grafos de 3-4 linhas. Sem floreio, sem "vamos juntos".

## 5. Estrutura completa (5 trilhas Â· 16 mÃ³dulos Â· 6 tÃ³picos cada)

> Cada mÃ³dulo: pÃ¡gina `modulo-X-Y.html` (500-800 linhas, 6-8 seÃ§Ãµes, â‰¥1 SVG, variedade de componentes) **e** entrada no index da trilha (accordion de 6 tÃ³picos Ã— 3 seÃ§Ãµes "O que Ã© / Por que aprender / Conceitos-chave"). Cada mÃ³dulo fecha com uma **MissÃ£o**.

### T1 â€” Fundamentos & Setup (Emerald) Â· NÃ­vel Aprendiz Â· 3 mÃ³dulos
**M1.1 â€” A oportunidade: IA + consultoria agora**
1. Por que 2026 Ã© o momento (dados de mercado â€” usar pesquisa)
2. O que Ã© estratÃ©gia/consultoria de IA na prÃ¡tica
3. A tese "entrada mÃ­nima, saÃ­da mÃ¡xima"
4. Da ferramenta Ã  renda (uso pessoal / na empresa / cliente pago)
5. O mito do "preciso ser programador"
6. Como o curso funciona (nÃ­veis, missÃµes, recursos)
*MissÃ£o:* escrever sua "tese de consultor" em 3 frases (nicho + dor + oferta).

**M1.2 â€” Anatomia da FÃ¡brica**
1. Os 19 entregÃ¡veis (panorama)
2. O pipeline de 3 fases (Pesquisa â†’ SÃ­ntese â†’ GeraÃ§Ã£o)
3. O que cada fase faz e por quÃª
4. Por que o output parece consultoria de elite (BCG/KPMG)
5. DemonstraÃ§Ã£o: um pacote real, peÃ§a por peÃ§a
6. O mapa do curso (o que vocÃª vai construir atÃ© o capstone)
*MissÃ£o:* listar, para uma empresa que vocÃª conhece, 3 entregÃ¡veis que mais venderiam.

**M1.3 â€” Montando o arsenal (setup)**
1. Claude Code: seu copiloto de construÃ§Ã£o
2. Conta + chave Perplexity (pesquisa ao vivo)
3. Conta + chave Gemini (sÃ­ntese barata, contexto gigante)
4. Clonar e rodar o repo (`linnoff88-dev/ai-strategy-factory`)
5. Build in public: a mentalidade (mostrar a bagunÃ§a, nÃ£o sÃ³ o resultado)
6. GestÃ£o de custo: quick vs deep, ~US$1, dividir pedidos
*MissÃ£o:* rodar a FÃ¡brica em modo quick para 1 empresa e abrir os arquivos.

### T2 â€” SÃ­ntese de Conhecimento (Blue) Â· NÃ­vel Sintetizador Â· 3 mÃ³dulos
**M2.1 â€” Os frameworks que valem ouro** (fonte: TLDRs + prompts reais)
1. AI Maturity Assessment (escala 1-5, readiness)
2. Quick Wins (matriz esforÃ§o Ã— impacto)
3. Build vs Buy (decisÃ£o de fornecedor)
4. ROI de IA (custo-benefÃ­cio, projeÃ§Ãµes)
5. Roadmap 30/60/90/180/360 dias
6. GovernanÃ§a de dados & polÃ­tica de uso aceitÃ¡vel
*MissÃ£o:* aplicar Quick Wins a um setor e listar 3 vitÃ³rias rÃ¡pidas.

**M2.2 â€” RAG preguiÃ§oso: PDF gigante â†’ cheat sheet** (fonte: `pdf_to_cheatsheet.py`, Fase 1)
1. O problema do contexto (PDFs de 28-46 pÃ¡ginas estouram o limite)
2. Chunking em blocos de ~10k tokens
3. O prompt de sÃ­ntese (extrair sÃ³ o valioso; cortar buzzword)
4. Gemini 2.5 Flash: barato e com contexto gigante
5. Montar o cheat sheet ultra-comprimido
6. `pdf_to_cheatsheet.py` na prÃ¡tica
*MissÃ£o:* transformar 1 PDF de consultoria num cheat sheet de 1 pÃ¡gina.

**M2.3 â€” Seu cÃ©rebro de consultor (base de conhecimento)**
1. Por que destilar conhecimento (token Ã© barato, contexto Ã© caro)
2. Curar fontes (McKinsey, BCG, KPMG, OpenAI, IBM)
3. Anatomia de um cheat sheet reutilizÃ¡vel
4. Versionar e organizar a base
5. Injetar contexto sem estourar tokens (RAG preguiÃ§oso aplicado)
6. Sua biblioteca pessoal de consultor
*MissÃ£o:* montar uma pasta `conhecimento/` com 3 cheat sheets curados.

### T3 â€” Skills & Agentes (Purple) Â· NÃ­vel Construtor Â· 4 mÃ³dulos
**M3.1 â€” Skills e subagentes: o que sÃ£o e quando usar**
1. O que Ã© uma skill (capacidade reutilizÃ¡vel, sob demanda)
2. O que Ã© um subagente (trabalho isolado, contexto prÃ³prio)
3. Skill vs agente: quando cada um
4. Anatomia de uma skill (`SKILL.md`, frontmatter `name`/`description`)
5. Onde skills e agentes vivem no Claude Code
6. O ecossistema de recursos reutilizÃ¡veis (por que isso vira ativo)
*MissÃ£o:* mapear 3 tarefas suas que viram skill e 2 que viram agente.

**M3.2 â€” Construa sua primeira skill (`diagnostico-ia`)**
1. Definir o gatilho (a `description` que faz a skill disparar)
2. Escrever o corpo (passos claros, determinÃ­sticos)
3. Anexar referÃªncias (os cheat sheets da T2)
4. Testar a skill com um caso real
5. Iterar e empacotar
6. Versionar e compartilhar
*MissÃ£o:* skill `diagnostico-ia` rodando e cuspindo um mini-diagnÃ³stico.

**M3.3 â€” A skill de documentos (DocX/PPTX/Excel/PDF)** (fonte: `document-creation-skills.md`, Fase 2)
1. Por que gerar documentos programaticamente
2. `python-docx` â€” relatÃ³rios Word
3. `python-pptx` â€” apresentaÃ§Ãµes (RGBColor, layouts)
4. `openpyxl` â€” Excel com fÃ³rmulas e convenÃ§Ã£o de cores
5. `reportlab` â€” PDF (Platypus)
6. Empacotar como skill `gerar-entregavel`
*MissÃ£o:* gerar 1 `.docx` + 1 `.pptx` a partir de um markdown.

**M3.4 â€” Construa seu subagente (pesquisador & redator)**
1. Anatomia de um subagente (system prompt, ferramentas, saÃ­da)
2. O agente `pesquisador-empresa` (coleta contexto estruturado)
3. O agente `redator-estrategia` (rascunha entregÃ¡vel a partir de pesquisa + framework)
4. SaÃ­da estruturada (schema, JSON confiÃ¡vel)
5. Orquestrar skill + agentes juntos
6. Quando paralelizar agentes
*MissÃ£o:* agente `pesquisador-empresa` retornando um `CompanyContext` preenchido.

### T4 â€” A FÃ¡brica (Amber) Â· NÃ­vel Engenheiro Â· 3 mÃ³dulos
**M4.1 â€” Pesquisa ao vivo com Perplexity** (fonte: `query_templates.py`, Fase 3)
1. Por que pesquisa ao vivo (nÃ£o ficar estÃ¡tico/desatualizado)
2. Quick vs Deep (sonar / sonar-pro / deep-research) e custo
3. Contexto temporal (injetar a data atual nas queries)
4. As 9 categorias de query (empresa, setor, concorrÃªncia, tech, IA, dores, regulatÃ³rio, lideranÃ§a, notÃ­cias)
5. Agregar e tratar resultados (degradaÃ§Ã£o graciosa)
6. Montar o `ResearchOutput`
*MissÃ£o:* pesquisa quick estruturada de 1 empresa, 9 categorias.

**M4.2 â€” Os 15 prompts de entregÃ¡veis** (fonte: `synthesis/prompts/*.py`)
1. Anatomia de um prompt de entregÃ¡vel profissional
2. AvaliaÃ§Ã£o (tech inventory, pain points, maturity)
3. Planejamento (roadmap, quick wins, ROI)
4. ImplementaÃ§Ã£o (build vs buy, licenÃ§as, casos de uso)
5. GovernanÃ§a (polÃ­tica de IA, dados, gestÃ£o de mudanÃ§a)
6. Recursos (biblioteca de prompts, glossÃ¡rio) + adaptar ao PT-BR
*MissÃ£o:* adaptar 1 prompt de entregÃ¡vel e gerar o markdown.

**M4.3 â€” OrquestraÃ§Ã£o, retomada e diagramas que vendem** (fonte: ARCHITECTURE.md, `mermaid_diagrams.py`)
1. O orquestrador de pipeline (cada etapa confirma antes de seguir)
2. Checkpoints e `state.json` (progress tracking)
3. Retomar sessÃ£o quando o contexto enche
4. Mermaid: estado atual vs futuro
5. Renderizar Mermaid â†’ PNG (e usar eraser.io / `beautiful-mermaid`)
6. Empacotar o pacote completo para download
*MissÃ£o:* rodar a FÃ¡brica ponta a ponta e gerar os diagramas.

### T5 â€” Da FÃ¡brica ao Cliente (Teal) Â· NÃ­vel Consultor Â· 3 mÃ³dulos
**M5.1 â€” Frontend e empacotamento** (fonte: Fase 5, webapp)
1. A interface mÃ­nima (nome + descriÃ§Ã£o + profundidade + enviar)
2. Rodar a webapp local (localhost:8888)
3. Progresso em tempo real (SSE) e download dos assets
4. Organizar o pacote por pastas
5. Marca: deixar o entregÃ¡vel com a sua cara
6. Hospedar/entregar o pacote
*MissÃ£o:* gerar e empacotar um pacote com a sua identidade.

**M5.2 â€” Posicionamento, oferta e preÃ§o** (fonte: pesquisa de mercado)
1. Achar seu nicho (setor + dor especÃ­fica)
2. A oferta produtizada (diagnÃ³stico de IA como produto)
3. PrecificaÃ§Ã£o (custo < US$1 vs valor de mercado; faixas reais)
4. Formatos: projeto, retainer, produtizado
5. Conseguir os primeiros clientes (canais, prova)
6. Ã‰tica e expectativa (o que a FÃ¡brica Ã© e nÃ£o Ã©)
*MissÃ£o:* escrever sua oferta de 1 pÃ¡gina (nicho, entregÃ¡vel, preÃ§o).

**M5.3 â€” A apresentaÃ§Ã£o que fecha + Capstone**
1. O deck executivo (estrutura que decide)
2. O SOW / declaraÃ§Ã£o de trabalho (escopo, preÃ§o, prazo)
3. Conduzir a reuniÃ£o (do diagnÃ³stico ao prÃ³ximo passo)
4. ObjeÃ§Ãµes comuns e respostas
5. **Capstone:** FÃ¡brica rodando para um cliente real
6. PrÃ³ximos passos (evoluir a fÃ¡brica, novos entregÃ¡veis)
*MissÃ£o (capstone):* pacote completo + deck + SOW de uma empresa real.

## 6. Recursos reutilizÃ¡veis (`recursos/`)

Arquivos reais, prontos para copiar. Adaptados do repo (PT-BR), curados.

```
recursos/
â”œâ”€â”€ README.md                      # Ã­ndice + como usar cada recurso
â”œâ”€â”€ skills/
â”‚   â”œâ”€â”€ diagnostico-ia/SKILL.md    # diagnÃ³stico (maturity+quick wins+roadmap) de empresa descrita
â”‚   â””â”€â”€ gerar-entregavel/SKILL.md  # markdown â†’ .docx/.pptx (wrap document-creation)
â”œâ”€â”€ agentes/
â”‚   â”œâ”€â”€ pesquisador-empresa.md     # subagente: pesquisa â†’ CompanyContext estruturado
â”‚   â””â”€â”€ redator-estrategia.md      # subagente: pesquisa + framework â†’ entregÃ¡vel
â”œâ”€â”€ prompts/                       # 15 prompts de entregÃ¡veis em PT-BR (paste-ready)
â”‚   â”œâ”€â”€ 01-tech-inventory.md ... 15-glossario.md
â”œâ”€â”€ templates/
â”‚   â”œâ”€â”€ sow.md                     # statement of work PT-BR
â”‚   â”œâ”€â”€ deck-executivo.md          # outline do deck
â”‚   â”œâ”€â”€ roadmap-30-60-90.md
â”‚   â””â”€â”€ roi-calculator.md          # estrutura da planilha (convenÃ§Ã£o de cores)
â””â”€â”€ diagramas/
    â”œâ”€â”€ pipeline.mmd               # Mermaid do pipeline 3 fases
    â”œâ”€â”€ estado-atual-vs-futuro.mmd
    â””â”€â”€ README.md                  # eraser.io + beautiful-mermaid
```

## 7. Identidade visual

- **Emoji do curso:** ðŸ­
- **Nome:** "FÃ¡brica de EstratÃ©gia de IA â€” Vire Consultor de IA"
- **Cores por trilha:** T1 Emerald, T2 Blue, T3 Purple, T4 Amber, T5 Teal (sequÃªncia cromÃ¡tica ARCKHÉ).
- **EstÃ©tica:** dark premium, Tailwind via CDN, Inter, SVG inline futurista, light mode obrigatÃ³rio. Zero imagens raster nas pÃ¡ginas (PNG opcional via ARCKHÉimg sÃ³ como extra decorativo â€” nÃ£o substitui SVG).

## 8. Plano de publicaÃ§Ã£o

1. **Git:** `git init` em `/home/nmaldaner/projetos/aiestrategia`, `.gitignore` (ignora `_reference/`, `docs/fontes/`, `venv`), commits incrementais.
2. **Repo remoto:** criar `linnoff88-dev/aiestrategia` (pÃºblico) via `gh`, push `main`.
3. **GitHub Pages:** habilitar Pages na branch `main` (root). Adicionar `.nojekyll`. URL `https://linnoff88-dev.github.io/
4. **Portal ARCKHÉ AI** (`/home/nmaldaner/projetos/portal`):
   - `src/data/courses.ts` â†’ `platformsData` (ordem alfabÃ©tica, id = max+1): title "FÃ¡brica de EstratÃ©gia de IA â€” Vire Consultor de IA", icon ðŸ­, tags ['IA','Consultoria','Claude Code','EstratÃ©gia'], url Pages.
   - `updatesData` (topo): `{ date:'2026-06-14', title:'â€¦', type:'novo', url:â€¦ }`.
   - Trilha hardcoded em `Portal.tsx`/`PortalV2.tsx`: sÃ³ se encaixar numa trilha existente; senÃ£o, standalone.
   - Commit + push (Vercel faz deploy).

## 9. Checklist de build & conformidade `formato-curso`

Por pÃ¡gina (ver `CHECKLIST_REVISAO.md` + 17 erros crÃ­ticos):
- [ ] Nav completo idÃªntico em TODAS as pÃ¡ginas (logo + ARCKHÉ AI sky-400 + 5 botÃµes de trilha + theme toggle); trilha ativa destacada.
- [ ] Light mode CSS completo (4 partes + cor de acento da trilha + bordas dark suavizadas).
- [ ] BotÃµes `justify-start`; tÃ³picos com nÃºmero em cÃ­rculo; tÃ­tulo de mÃ³dulo `text-2xl`.
- [ ] Index de trilha: header + stats(4) + **Mapa da trilha** + "Conteudo detalhado" + cards de mÃ³dulo (cada um com 6-8 tÃ³picos accordion de 3 seÃ§Ãµes + "Ver em Modal" iframe + "Ver Completo").
- [ ] MÃ³dulo: breadcrumb + header stats(4) + 6-8 seÃ§Ãµes variadas (â‰¥2 grids âœ“/âœ—, â‰¥1 timeline, â‰¥2 tip boxes, code box quando Ãºtil) + â‰¥1 SVG futurista + Resumo final + MissÃ£o.
- [ ] Hero SVG no index de cada trilha.
- [ ] Tom ARCKHÉ; missÃµes com payoff concreto.

**Ordem de build:** (a) scaffold + git; (b) golden reference: `index.html` + `curso/index.html` + `curso/trilha1/index.html` + `curso/trilha1/modulo-1-1.html`; (c) fan-out por trilha (subagentes seguindo golden + este spec); (d) `recursos/`; (e) auditoria `revisar-curso` + fix; (f) publicaÃ§Ã£o.

## 10. Fontes

- Repo: `_reference/ai-strategy-factory/` (README, ARCHITECTURE.md, CLAUDE.md, `synthesis/prompts/*.py`, `research/query_templates.py`, `generation/*`, `Consulting Guides TLDR/*`, `.claude/document-creation-skills.md`).
- MÃ©todo: `docs/fontes/IA-metodologia.txt` (5 fases).
- Pesquisa de mercado: agente web (em curso) â€” dados/estatÃ­sticas para ganchos motivacionais e a trilha T5.
- Template: skill `formato-curso` (`MASTER_COMPLETO.md`, `SVG-FUTURISTA.md`, `DESIGN-SYSTEM.md`, `CHECKLIST_REVISAO.md`).
