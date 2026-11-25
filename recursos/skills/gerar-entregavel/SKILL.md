---
name: gerar-entregavel
description: >-
  Use quando o usuário quiser converter um entregável em markdown (diagnóstico,
  roadmap, política de IA, etc.) em arquivos finais .docx (Word) e .pptx
  (PowerPoint) prontos para entregar a um cliente. Acione com pedidos como
  "transforma esse markdown em Word e PowerPoint", "gera o .docx e o deck desse
  entregável", "exporta esse diagnóstico pra apresentar", "monta os documentos
  finais do pacote". É a peça de empacotamento da Fábrica de Estratégia de IA.
---

# Gerar entregável (.md → .docx + .pptx)

Recebe um markdown de entregável e gera os documentos finais com `python-docx`
e `python-pptx`. Saída padrêo em `~/projetos/output/<empresa>/` (ou onde o
usuário indicar): um `.docx` (relatório) e um `.pptx` (deck executivo).

## Setup (uma vez por máquina)

Crie um virtualenv para nêo conflitar com o Python do sistema:

```bash
python3 -m venv venv
source venv/bin/activate
pip install python-docx python-pptx openpyxl reportlab
```

`openpyxl` e `reportlab` entram porque o mesmo pacote costuma precisar de Excel
(ROI) e PDF; ver seções 3 e 4. Para só docx/pptx, bastam os dois primeiros.

## Passos (determinísticos)

### 1. Ler e parsear o markdown

Carregue o `.md` do entregável e mapeie a estrutura por heading:

- `#` → título do documento / slide de capa
- `##` → seçêo (heading nível 1 no docx / 1 slide no pptx)
- `###` → subseçêo (heading nível 2 / bullet de destaque)
- tabelas markdown → tabelas nativas
- listas `-` / `1.` → bullets / lista numerada

### 2. Gerar o .docx (relatório Word) com `python-docx`

```python
from docx import Document
from docx.shared import Pt, RGBColor
from docx.enum.text import WD_ALIGN_PARAGRAPH

doc = Document()

# Capa
title = doc.add_heading('Diagnóstico de IA — {Empresa}', level=0)
title.alignment = WD_ALIGN_PARAGRAPH.CENTER

# Seçêo (## vira heading 1)
doc.add_heading('Resumo executivo', level=1)
doc.add_paragraph('Texto do parágrafo.')

# Lista com marcadores
doc.add_paragraph('Primeira vitória rápida', style='List Bullet')

# Tabela (cabeçalho + linhas)
headers = ['#', 'Quick Win', 'Esforço', 'Impacto']
rows = [['1', 'Triagem de currículos', 'Baixo', 'Alto']]
table = doc.add_table(rows=1, cols=len(headers))
table.style = 'Table Grid'
for i, h in enumerate(headers):
    table.rows[0].cells[i].text = h
for row in rows:
    cells = table.add_row().cells
    for i, v in enumerate(row):
        cells[i].text = str(v)

# Texto formatado / cor (use RGBColor, NêO RgbColor)
p = doc.add_paragraph()
run = p.add_run('Destaque')
run.bold = True
run.font.size = Pt(12)
run.font.color.rgb = RGBColor(0x1F, 0x4E, 0x79)  # azul corporativo

doc.save('relatorio.docx')
```

Estilos úteis: `'List Bullet'`, `'List Number'`, `'Table Grid'`, `'Heading 1'`,
`'Heading 2'`.

### 3. Gerar o .pptx (deck executivo) com `python-pptx`

Um slide por seçêo `##`. Layout `6` (em branco) dá mais controle.

```python
from pptx import Presentation
from pptx.util import Inches, Pt
from pptx.dml.color import RGBColor   # GOTCHA: é RGBColor, nêo RgbColor
from pptx.enum.text import PP_ALIGN

prs = Presentation()
DARK_BLUE = RGBColor(31, 78, 121)

def slide_titulo(prs, titulo, subtitulo=''):
    s = prs.slides.add_slide(prs.slide_layouts[6])  # blank
    tb = s.shapes.add_textbox(Inches(0.5), Inches(2.4), Inches(9), Inches(1.5))
    tf = tb.text_frame; tf.word_wrap = True
    p = tf.paragraphs[0]; p.text = titulo
    p.font.size = Pt(40); p.font.bold = True
    p.font.color.rgb = DARK_BLUE; p.alignment = PP_ALIGN.CENTER
    return s

def slide_bullets(prs, titulo, bullets):
    s = prs.slides.add_slide(prs.slide_layouts[6])
    # título
    th = s.shapes.add_textbox(Inches(0.5), Inches(0.4), Inches(9), Inches(1))
    tp = th.text_frame.paragraphs[0]; tp.text = titulo
    tp.font.size = Pt(28); tp.font.bold = True; tp.font.color.rgb = DARK_BLUE
    # corpo
    bb = s.shapes.add_textbox(Inches(0.7), Inches(1.6), Inches(8.6), Inches(5))
    tf = bb.text_frame; tf.word_wrap = True
    for i, b in enumerate(bullets):
        p = tf.paragraphs[0] if i == 0 else tf.add_paragraph()
        p.text = f'• {b}'; p.font.size = Pt(20); p.space_after = Pt(10)
    return s

slide_titulo(prs, 'Diagnóstico de IA — {Empresa}', '{data}')
slide_bullets(prs, 'Resumo executivo',
              ['Maturidade: nível 2/5', '5 vitórias rápidas', 'Roadmap 30/60/90'])
prs.save('deck.pptx')
```

Para tabelas no pptx use `slide.shapes.add_table(rows, cols, left, top, w, h).table`
e preencha com `table.cell(r, c).text`.

### 4. (Opcional) Excel de ROI e PDF

Se o entregável for o calculador de ROI, gere `.xlsx` com `openpyxl` seguindo
a estrutura de `templates/roi-calculator.md`. Para PDF, use `reportlab`
(Platypus: `SimpleDocTemplate` + `story` + `doc.build(story)`).

### 5. Salvar e reportar

Salve em `~/projetos/output/<empresa>/documentos/` (crie a pasta). Reporte os
caminhos absolutos dos arquivos gerados.

## Gotchas (decorar)

- **python-pptx:** importe `RGBColor`, **nêo** `RgbColor`.
- **openpyxl:** indexaçêo é **1-based** (`row=1, column=1` é a célula `A1`).
  Sempre use **fórmulas** (`ws['E5'] = '=SUM(B5:D5)'`), nunca grave o valor
  calculado na mêo.
- **reportlab:** o PDF só é escrito no fim, com `doc.build(story)`.
- **Cores Excel (convençêo de modelo financeiro):** azul `0000FF` = input do
  usuário; preto `000000` = fórmula; verde `008000` = link entre abas; vermelho
  `FF0000` = referência externa; fundo amarelo `FFFF00` = premissa-chave.
- **Todos:** sempre dentro do `venv`, senêo conflita com o Python do sistema.

## Critério de sucesso

Abrir o `.docx` e o `.pptx` gerados e ver o entregável fielmente convertido
(títulos, seções, tabelas, bullets), pronto para enviar ao cliente.
