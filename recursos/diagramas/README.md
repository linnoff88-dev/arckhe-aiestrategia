# Diagramas (Mermaid)

Diagramas que **vendem**: estado atual vs futuro, pipeline, roadmap visual.
Ficam em texto (`.mmd`) e viram imagem para entrar no `.docx`/`.pptx` ou na
página do entregável.

## Arquivos

- `pipeline.mmd` — o pipeline de 3 fases da Fábrica (Pesquisa → Síntese →
  Geração). Use no M1.2 / M4.3 para explicar a arquitetura.
- `estado-atual-vs-futuro.mmd` — exemplo de arquitetura **atual** vs **futura
  (habilitada por IA)** de uma empresa. Adapte os blocos ao cliente; é o
  diagrama-âncora do diagnóstico.

## Como renderizar

Três caminhos, do mais rápido ao mais integrado:

1. **mermaid.live** — cole o conteúdo do `.mmd`, baixe SVG/PNG. Bom para um
   diagrama avulso e rápido. <https://mermaid.live>
2. **eraser.io** — gerador de diagrama Mermaid gratuito, com ajuste visual e
   export limpo. Bom quando o diagrama vai para um deck de cliente.
   <https://www.eraser.io/make/free-mermaid-diagram-maker>
3. **skill `beautiful-mermaid`** — renderiza o Mermaid como SVG **e** PNG
   localmente, com estética caprichada. Use dentro do Claude Code quando quiser
   o PNG já no pacote, sem sair pro navegador. Peça: "renderiza esse diagrama
   Mermaid".

## Como usar nos entregáveis

- **No `.pptx`/`.docx`:** renderize para **PNG** (eraser.io ou
  `beautiful-mermaid`) e insira a imagem. `python-pptx`/`python-docx` colocam
  imagem com `add_picture(...)`.
- **Na página do entregável (HTML):** dá para embutir o Mermaid e deixar o
  navegador renderizar, ou usar o SVG exportado.
- **Convenção de cores:** marque gargalos/dores do estado atual em vermelho
  (classe `warn` no exemplo) e a camada de IA do estado futuro na cor de
  destaque do entregável. Isso cria o contraste "antes × depois" que fecha
  reunião.

## Dica de fidelidade

O prompt `03-diagramas.md` (em `recursos/prompts/`) gera o **código Mermaid**
a partir da pesquisa. Fluxo: prompt `03` produz o `.mmd` → renderiza aqui →
imagem entra no pacote.
