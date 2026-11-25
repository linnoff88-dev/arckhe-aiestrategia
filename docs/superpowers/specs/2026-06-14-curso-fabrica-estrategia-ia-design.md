# Curso: FêÂ¡brica de EstratêÂ©gia de IA ê¢â¬â Vire Consultor de IA

> **Spec / Blueprint** ê¢â¬â fonte êÂºnica de verdade para o build.
> **Data:** 2026-06-14 êÂ· **Formato:** ARCKHê AI (skill `formato-curso`) êÂ· **Idioma:** PT-BR
> **Repo:** `linnoff88-dev/aiestrategia` ê¢â â `https://linnoff88-dev.github.io/ êÂ· **Portal:** ARCKHê AI

---

## 1. Resumo executivo

Curso prêÂ¡tico, mêÂ£o na massa, para quem quer **entrar na êÂ¡rea de IA e de consultoria de IA**. O aluno **constrêÂ³i a prêÂ³pria FêÂ¡brica de EstratêÂ©gia de IA** (uma ferramenta que gera pacotes de consultoria ê¢â¬â 19 entregêÂ¡veis ê¢â¬â automaticamente, com Claude Code + Perplexity + Gemini) e, no mesmo movimento, aprende a **se posicionar e vender como consultor**. Cada habilidade têÂ©cnica êÂ© enquadrada como uma capacidade vendêÂ¡vel.

**Promessa:** sair do zero e terminar com (1) uma fêÂ¡brica funcionando, (2) um arsenal de skills/agentes/prompts reutilizêÂ¡veis, e (3) um primeiro entregêÂ¡vel de consultoria pronto para apresentar a um cliente real.

**Tese central (do material-fonte):** *entrada mêÂ­nima, saêÂ­da mêÂ¡xima*. Duas caixas de texto ê¢â â pacote de consultoria impecêÂ¡vel. Custo < US$1, valor de mercado de milhares.

## 2. PêÂºblico & objetivos

- **PêÂºblico:** iniciante a intermediêÂ¡rio, **nêÂ£o exige ser dev**. Orquestra tudo via Claude Code.
- **Objetivo de aprendizagem:** rêÂ¡pido mas completo ê¢â¬â do conceito ao entregêÂ¡vel vendêÂ¡vel.
- **Resultado final (capstone):** rodar a FêÂ¡brica para uma empresa real e montar a apresentaêÂ§êÂ£o + SOW.

## 3. êângulo & decisêÂµes

- **êângulo C (hêÂ­brido):** espinha = construir a FêÂ¡brica (as 5 fases do material-fonte `IA-metodologia.txt`); camada de negêÂ³cio enquadra cada habilidade como serviêÂ§o de consultoria; fecha com trilha de entrega/venda + capstone.
- **Fonte de conteêÂºdo:** repo `ai-strategy-factory` (cêÂ³digo real, 15 prompts, TLDRs BCG/KPMG/McKinsey) + `IA-metodologia.txt` (mêÂ©todo das 5 fases) + pesquisa de mercado.
- **Fidelidade:** referenciar sempre o repo do usuêÂ¡rio (`linnoff88-dev/ai-strategy-factory`), nêÂ£o o upstream.

## 4. MecêÂ¢nica pedagêÂ³gica

### 4.1 Sistema de nêÂ­veis (subir de nêÂ­vel)
Cada trilha êÂ© um **nêÂ­vel** com badge. O index (landing) mostra a progressêÂ£o.

| NêÂ­vel | Badge | Trilha | Cor |
|---|---|---|---|
| 1. Aprendiz | ê°Å¸Â¥â° | Fundamentos & Setup | Emerald (T1) |
| 2. Sintetizador | ê°Å¸Â¥Ë | SêÂ­ntese de Conhecimento | Blue (T2) |
| 3. Construtor | ê°Å¸Â¥â¡ | Skills & Agentes | Purple (T3) |
| 4. Engenheiro | ê°Å¸âÅ½ | A FêÂ¡brica | Amber (T4) |
| 5. Consultor | ê°Å¸ââ | Da FêÂ¡brica ao Cliente | Teal (T5) |

### 4.2 MissêÂµes (exercêÂ­cios)
Cada mêÂ³dulo termina com uma **MissêÂ£o**: tarefa curta com **vitêÂ³ria concreta** e um **artefato que o aluno leva**. PadrêÂ£o de copy: "Ao fim vocêÂª tem **X funcionando** e pode **cobrar Y por isso**." Sem coachzinho (regra de tom ARCKHê): motivaêÂ§êÂ£o vem do **payoff concreto** e da **progressêÂ£o de nêÂ­vel**, nêÂ£o de exclamaêÂ§êÂ£o.

- Cada MissêÂ£o: objetivo (1 frase) ê¢â â passos (3-5) ê¢â â critêÂ©rio de sucesso verificêÂ¡vel ê¢â â "o que vocêÂª ganhou".
- **Desafio relêÂ¢mpago** opcional por trilha (mais difêÂ­cil, marca de maestria).

### 4.3 Recursos reutilizêÂ¡veis (entregêÂ¡veis do curso)
Pasta `recursos/` no repo, com skills, agentes, prompts e templates prontos para copiar e usar (detalhe na êÂ§6). êâ° o cumprimento do pedido "exemplos prêÂ¡ticos facilmente utilizêÂ¡veis, criando skills, agentes e outros recursos".

### 4.4 Diagramas
- **Dentro das pêÂ¡ginas:** cada mêÂ³dulo de conteêÂºdo tem ê¢â°Â¥1 **SVG futurista inline** (regra `formato-curso` #17) na cor da trilha + ciano.
- **Como conteêÂºdo ensinado:** Mermaid (estado atual vs futuro), com `recursos/diagramas/` e ponteiros para **eraser.io** e a skill `beautiful-mermaid`.

### 4.5 Tom de voz (ARCKHê)
Direto, brasileiro ("vocêÂª"), concreto (nêÂºmeros, R$, %), sêÂ³brio. ParêÂ¡grafos de 3-4 linhas. Sem floreio, sem "vamos juntos".

## 5. Estrutura completa (5 trilhas êÂ· 16 mêÂ³dulos êÂ· 6 têÂ³picos cada)

> Cada mêÂ³dulo: pêÂ¡gina `modulo-X-Y.html` (500-800 linhas, 6-8 seêÂ§êÂµes, ê¢â°Â¥1 SVG, variedade de componentes) **e** entrada no index da trilha (accordion de 6 têÂ³picos êâ 3 seêÂ§êÂµes "O que êÂ© / Por que aprender / Conceitos-chave"). Cada mêÂ³dulo fecha com uma **MissêÂ£o**.

### T1 ê¢â¬â Fundamentos & Setup (Emerald) êÂ· NêÂ­vel Aprendiz êÂ· 3 mêÂ³dulos
**M1.1 ê¢â¬â A oportunidade: IA + consultoria agora**
1. Por que 2026 êÂ© o momento (dados de mercado ê¢â¬â usar pesquisa)
2. O que êÂ© estratêÂ©gia/consultoria de IA na prêÂ¡tica
3. A tese "entrada mêÂ­nima, saêÂ­da mêÂ¡xima"
4. Da ferramenta êÂ  renda (uso pessoal / na empresa / cliente pago)
5. O mito do "preciso ser programador"
6. Como o curso funciona (nêÂ­veis, missêÂµes, recursos)
*MissêÂ£o:* escrever sua "tese de consultor" em 3 frases (nicho + dor + oferta).

**M1.2 ê¢â¬â Anatomia da FêÂ¡brica**
1. Os 19 entregêÂ¡veis (panorama)
2. O pipeline de 3 fases (Pesquisa ê¢â â SêÂ­ntese ê¢â â GeraêÂ§êÂ£o)
3. O que cada fase faz e por quêÂª
4. Por que o output parece consultoria de elite (BCG/KPMG)
5. DemonstraêÂ§êÂ£o: um pacote real, peêÂ§a por peêÂ§a
6. O mapa do curso (o que vocêÂª vai construir atêÂ© o capstone)
*MissêÂ£o:* listar, para uma empresa que vocêÂª conhece, 3 entregêÂ¡veis que mais venderiam.

**M1.3 ê¢â¬â Montando o arsenal (setup)**
1. Claude Code: seu copiloto de construêÂ§êÂ£o
2. Conta + chave Perplexity (pesquisa ao vivo)
3. Conta + chave Gemini (sêÂ­ntese barata, contexto gigante)
4. Clonar e rodar o repo (`linnoff88-dev/ai-strategy-factory`)
5. Build in public: a mentalidade (mostrar a bagunêÂ§a, nêÂ£o sêÂ³ o resultado)
6. GestêÂ£o de custo: quick vs deep, ~US$1, dividir pedidos
*MissêÂ£o:* rodar a FêÂ¡brica em modo quick para 1 empresa e abrir os arquivos.

### T2 ê¢â¬â SêÂ­ntese de Conhecimento (Blue) êÂ· NêÂ­vel Sintetizador êÂ· 3 mêÂ³dulos
**M2.1 ê¢â¬â Os frameworks que valem ouro** (fonte: TLDRs + prompts reais)
1. AI Maturity Assessment (escala 1-5, readiness)
2. Quick Wins (matriz esforêÂ§o êâ impacto)
3. Build vs Buy (decisêÂ£o de fornecedor)
4. ROI de IA (custo-benefêÂ­cio, projeêÂ§êÂµes)
5. Roadmap 30/60/90/180/360 dias
6. GovernanêÂ§a de dados & polêÂ­tica de uso aceitêÂ¡vel
*MissêÂ£o:* aplicar Quick Wins a um setor e listar 3 vitêÂ³rias rêÂ¡pidas.

**M2.2 ê¢â¬â RAG preguiêÂ§oso: PDF gigante ê¢â â cheat sheet** (fonte: `pdf_to_cheatsheet.py`, Fase 1)
1. O problema do contexto (PDFs de 28-46 pêÂ¡ginas estouram o limite)
2. Chunking em blocos de ~10k tokens
3. O prompt de sêÂ­ntese (extrair sêÂ³ o valioso; cortar buzzword)
4. Gemini 2.5 Flash: barato e com contexto gigante
5. Montar o cheat sheet ultra-comprimido
6. `pdf_to_cheatsheet.py` na prêÂ¡tica
*MissêÂ£o:* transformar 1 PDF de consultoria num cheat sheet de 1 pêÂ¡gina.

**M2.3 ê¢â¬â Seu cêÂ©rebro de consultor (base de conhecimento)**
1. Por que destilar conhecimento (token êÂ© barato, contexto êÂ© caro)
2. Curar fontes (McKinsey, BCG, KPMG, OpenAI, IBM)
3. Anatomia de um cheat sheet reutilizêÂ¡vel
4. Versionar e organizar a base
5. Injetar contexto sem estourar tokens (RAG preguiêÂ§oso aplicado)
6. Sua biblioteca pessoal de consultor
*MissêÂ£o:* montar uma pasta `conhecimento/` com 3 cheat sheets curados.

### T3 ê¢â¬â Skills & Agentes (Purple) êÂ· NêÂ­vel Construtor êÂ· 4 mêÂ³dulos
**M3.1 ê¢â¬â Skills e subagentes: o que sêÂ£o e quando usar**
1. O que êÂ© uma skill (capacidade reutilizêÂ¡vel, sob demanda)
2. O que êÂ© um subagente (trabalho isolado, contexto prêÂ³prio)
3. Skill vs agente: quando cada um
4. Anatomia de uma skill (`SKILL.md`, frontmatter `name`/`description`)
5. Onde skills e agentes vivem no Claude Code
6. O ecossistema de recursos reutilizêÂ¡veis (por que isso vira ativo)
*MissêÂ£o:* mapear 3 tarefas suas que viram skill e 2 que viram agente.

**M3.2 ê¢â¬â Construa sua primeira skill (`diagnostico-ia`)**
1. Definir o gatilho (a `description` que faz a skill disparar)
2. Escrever o corpo (passos claros, determinêÂ­sticos)
3. Anexar referêÂªncias (os cheat sheets da T2)
4. Testar a skill com um caso real
5. Iterar e empacotar
6. Versionar e compartilhar
*MissêÂ£o:* skill `diagnostico-ia` rodando e cuspindo um mini-diagnêÂ³stico.

**M3.3 ê¢â¬â A skill de documentos (DocX/PPTX/Excel/PDF)** (fonte: `document-creation-skills.md`, Fase 2)
1. Por que gerar documentos programaticamente
2. `python-docx` ê¢â¬â relatêÂ³rios Word
3. `python-pptx` ê¢â¬â apresentaêÂ§êÂµes (RGBColor, layouts)
4. `openpyxl` ê¢â¬â Excel com fêÂ³rmulas e convenêÂ§êÂ£o de cores
5. `reportlab` ê¢â¬â PDF (Platypus)
6. Empacotar como skill `gerar-entregavel`
*MissêÂ£o:* gerar 1 `.docx` + 1 `.pptx` a partir de um markdown.

**M3.4 ê¢â¬â Construa seu subagente (pesquisador & redator)**
1. Anatomia de um subagente (system prompt, ferramentas, saêÂ­da)
2. O agente `pesquisador-empresa` (coleta contexto estruturado)
3. O agente `redator-estrategia` (rascunha entregêÂ¡vel a partir de pesquisa + framework)
4. SaêÂ­da estruturada (schema, JSON confiêÂ¡vel)
5. Orquestrar skill + agentes juntos
6. Quando paralelizar agentes
*MissêÂ£o:* agente `pesquisador-empresa` retornando um `CompanyContext` preenchido.

### T4 ê¢â¬â A FêÂ¡brica (Amber) êÂ· NêÂ­vel Engenheiro êÂ· 3 mêÂ³dulos
**M4.1 ê¢â¬â Pesquisa ao vivo com Perplexity** (fonte: `query_templates.py`, Fase 3)
1. Por que pesquisa ao vivo (nêÂ£o ficar estêÂ¡tico/desatualizado)
2. Quick vs Deep (sonar / sonar-pro / deep-research) e custo
3. Contexto temporal (injetar a data atual nas queries)
4. As 9 categorias de query (empresa, setor, concorrêÂªncia, tech, IA, dores, regulatêÂ³rio, lideranêÂ§a, notêÂ­cias)
5. Agregar e tratar resultados (degradaêÂ§êÂ£o graciosa)
6. Montar o `ResearchOutput`
*MissêÂ£o:* pesquisa quick estruturada de 1 empresa, 9 categorias.

**M4.2 ê¢â¬â Os 15 prompts de entregêÂ¡veis** (fonte: `synthesis/prompts/*.py`)
1. Anatomia de um prompt de entregêÂ¡vel profissional
2. AvaliaêÂ§êÂ£o (tech inventory, pain points, maturity)
3. Planejamento (roadmap, quick wins, ROI)
4. ImplementaêÂ§êÂ£o (build vs buy, licenêÂ§as, casos de uso)
5. GovernanêÂ§a (polêÂ­tica de IA, dados, gestêÂ£o de mudanêÂ§a)
6. Recursos (biblioteca de prompts, glossêÂ¡rio) + adaptar ao PT-BR
*MissêÂ£o:* adaptar 1 prompt de entregêÂ¡vel e gerar o markdown.

**M4.3 ê¢â¬â OrquestraêÂ§êÂ£o, retomada e diagramas que vendem** (fonte: ARCHITECTURE.md, `mermaid_diagrams.py`)
1. O orquestrador de pipeline (cada etapa confirma antes de seguir)
2. Checkpoints e `state.json` (progress tracking)
3. Retomar sessêÂ£o quando o contexto enche
4. Mermaid: estado atual vs futuro
5. Renderizar Mermaid ê¢â â PNG (e usar eraser.io / `beautiful-mermaid`)
6. Empacotar o pacote completo para download
*MissêÂ£o:* rodar a FêÂ¡brica ponta a ponta e gerar os diagramas.

### T5 ê¢â¬â Da FêÂ¡brica ao Cliente (Teal) êÂ· NêÂ­vel Consultor êÂ· 3 mêÂ³dulos
**M5.1 ê¢â¬â Frontend e empacotamento** (fonte: Fase 5, webapp)
1. A interface mêÂ­nima (nome + descriêÂ§êÂ£o + profundidade + enviar)
2. Rodar a webapp local (localhost:8888)
3. Progresso em tempo real (SSE) e download dos assets
4. Organizar o pacote por pastas
5. Marca: deixar o entregêÂ¡vel com a sua cara
6. Hospedar/entregar o pacote
*MissêÂ£o:* gerar e empacotar um pacote com a sua identidade.

**M5.2 ê¢â¬â Posicionamento, oferta e preêÂ§o** (fonte: pesquisa de mercado)
1. Achar seu nicho (setor + dor especêÂ­fica)
2. A oferta produtizada (diagnêÂ³stico de IA como produto)
3. PrecificaêÂ§êÂ£o (custo < US$1 vs valor de mercado; faixas reais)
4. Formatos: projeto, retainer, produtizado
5. Conseguir os primeiros clientes (canais, prova)
6. êâ°tica e expectativa (o que a FêÂ¡brica êÂ© e nêÂ£o êÂ©)
*MissêÂ£o:* escrever sua oferta de 1 pêÂ¡gina (nicho, entregêÂ¡vel, preêÂ§o).

**M5.3 ê¢â¬â A apresentaêÂ§êÂ£o que fecha + Capstone**
1. O deck executivo (estrutura que decide)
2. O SOW / declaraêÂ§êÂ£o de trabalho (escopo, preêÂ§o, prazo)
3. Conduzir a reuniêÂ£o (do diagnêÂ³stico ao prêÂ³ximo passo)
4. ObjeêÂ§êÂµes comuns e respostas
5. **Capstone:** FêÂ¡brica rodando para um cliente real
6. PrêÂ³ximos passos (evoluir a fêÂ¡brica, novos entregêÂ¡veis)
*MissêÂ£o (capstone):* pacote completo + deck + SOW de uma empresa real.

## 6. Recursos reutilizêÂ¡veis (`recursos/`)

Arquivos reais, prontos para copiar. Adaptados do repo (PT-BR), curados.

```
recursos/
ê¢âÅê¢ââ¬ê¢ââ¬ README.md                      # êÂ­ndice + como usar cada recurso
ê¢âÅê¢ââ¬ê¢ââ¬ skills/
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ diagnostico-ia/SKILL.md    # diagnêÂ³stico (maturity+quick wins+roadmap) de empresa descrita
ê¢ââ   ê¢ââê¢ââ¬ê¢ââ¬ gerar-entregavel/SKILL.md  # markdown ê¢â â .docx/.pptx (wrap document-creation)
ê¢âÅê¢ââ¬ê¢ââ¬ agentes/
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ pesquisador-empresa.md     # subagente: pesquisa ê¢â â CompanyContext estruturado
ê¢ââ   ê¢ââê¢ââ¬ê¢ââ¬ redator-estrategia.md      # subagente: pesquisa + framework ê¢â â entregêÂ¡vel
ê¢âÅê¢ââ¬ê¢ââ¬ prompts/                       # 15 prompts de entregêÂ¡veis em PT-BR (paste-ready)
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ 01-tech-inventory.md ... 15-glossario.md
ê¢âÅê¢ââ¬ê¢ââ¬ templates/
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ sow.md                     # statement of work PT-BR
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ deck-executivo.md          # outline do deck
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ roadmap-30-60-90.md
ê¢ââ   ê¢ââê¢ââ¬ê¢ââ¬ roi-calculator.md          # estrutura da planilha (convenêÂ§êÂ£o de cores)
ê¢ââê¢ââ¬ê¢ââ¬ diagramas/
    ê¢âÅê¢ââ¬ê¢ââ¬ pipeline.mmd               # Mermaid do pipeline 3 fases
    ê¢âÅê¢ââ¬ê¢ââ¬ estado-atual-vs-futuro.mmd
    ê¢ââê¢ââ¬ê¢ââ¬ README.md                  # eraser.io + beautiful-mermaid
```

## 7. Identidade visual

- **Emoji do curso:** ê°Å¸ÂÂ­
- **Nome:** "FêÂ¡brica de EstratêÂ©gia de IA ê¢â¬â Vire Consultor de IA"
- **Cores por trilha:** T1 Emerald, T2 Blue, T3 Purple, T4 Amber, T5 Teal (sequêÂªncia cromêÂ¡tica ARCKHê).
- **EstêÂ©tica:** dark premium, Tailwind via CDN, Inter, SVG inline futurista, light mode obrigatêÂ³rio. Zero imagens raster nas pêÂ¡ginas (PNG opcional via ARCKHêimg sêÂ³ como extra decorativo ê¢â¬â nêÂ£o substitui SVG).

## 8. Plano de publicaêÂ§êÂ£o

1. **Git:** `git init` em `/home/nmaldaner/projetos/aiestrategia`, `.gitignore` (ignora `_reference/`, `docs/fontes/`, `venv`), commits incrementais.
2. **Repo remoto:** criar `linnoff88-dev/aiestrategia` (pêÂºblico) via `gh`, push `main`.
3. **GitHub Pages:** habilitar Pages na branch `main` (root). Adicionar `.nojekyll`. URL `https://linnoff88-dev.github.io/
4. **Portal ARCKHê AI** (`/home/nmaldaner/projetos/portal`):
   - `src/data/courses.ts` ê¢â â `platformsData` (ordem alfabêÂ©tica, id = max+1): title "FêÂ¡brica de EstratêÂ©gia de IA ê¢â¬â Vire Consultor de IA", icon ê°Å¸ÂÂ­, tags ['IA','Consultoria','Claude Code','EstratêÂ©gia'], url Pages.
   - `updatesData` (topo): `{ date:'2026-06-14', title:'ê¢â¬Â¦', type:'novo', url:ê¢â¬Â¦ }`.
   - Trilha hardcoded em `Portal.tsx`/`PortalV2.tsx`: sêÂ³ se encaixar numa trilha existente; senêÂ£o, standalone.
   - Commit + push (Vercel faz deploy).

## 9. Checklist de build & conformidade `formato-curso`

Por pêÂ¡gina (ver `CHECKLIST_REVISAO.md` + 17 erros crêÂ­ticos):
- [ ] Nav completo idêÂªntico em TODAS as pêÂ¡ginas (logo + ARCKHê AI sky-400 + 5 botêÂµes de trilha + theme toggle); trilha ativa destacada.
- [ ] Light mode CSS completo (4 partes + cor de acento da trilha + bordas dark suavizadas).
- [ ] BotêÂµes `justify-start`; têÂ³picos com nêÂºmero em cêÂ­rculo; têÂ­tulo de mêÂ³dulo `text-2xl`.
- [ ] Index de trilha: header + stats(4) + **Mapa da trilha** + "Conteudo detalhado" + cards de mêÂ³dulo (cada um com 6-8 têÂ³picos accordion de 3 seêÂ§êÂµes + "Ver em Modal" iframe + "Ver Completo").
- [ ] MêÂ³dulo: breadcrumb + header stats(4) + 6-8 seêÂ§êÂµes variadas (ê¢â°Â¥2 grids ê¢Åâ/ê¢Åâ, ê¢â°Â¥1 timeline, ê¢â°Â¥2 tip boxes, code box quando êÂºtil) + ê¢â°Â¥1 SVG futurista + Resumo final + MissêÂ£o.
- [ ] Hero SVG no index de cada trilha.
- [ ] Tom ARCKHê; missêÂµes com payoff concreto.

**Ordem de build:** (a) scaffold + git; (b) golden reference: `index.html` + `curso/index.html` + `curso/trilha1/index.html` + `curso/trilha1/modulo-1-1.html`; (c) fan-out por trilha (subagentes seguindo golden + este spec); (d) `recursos/`; (e) auditoria `revisar-curso` + fix; (f) publicaêÂ§êÂ£o.

## 10. Fontes

- Repo: `_reference/ai-strategy-factory/` (README, ARCHITECTURE.md, CLAUDE.md, `synthesis/prompts/*.py`, `research/query_templates.py`, `generation/*`, `Consulting Guides TLDR/*`, `.claude/document-creation-skills.md`).
- MêÂ©todo: `docs/fontes/IA-metodologia.txt` (5 fases).
- Pesquisa de mercado: agente web (em curso) ê¢â¬â dados/estatêÂ­sticas para ganchos motivacionais e a trilha T5.
- Template: skill `formato-curso` (`MASTER_COMPLETO.md`, `SVG-FUTURISTA.md`, `DESIGN-SYSTEM.md`, `CHECKLIST_REVISAO.md`).
