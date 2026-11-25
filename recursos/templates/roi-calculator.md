# Calculadora de ROI — estrutura da planilha

> Especificaçêo da planilha (.xlsx) de ROI de IA. Descreve abas, linhas/colunas,
> fórmulas e a convençêo de cores. Gere com `openpyxl` (skill `gerar-entregavel`).
> Regra de ouro: **valores calculados sêo fórmulas, nunca números digitados**.

---

## Convençêo de cores (modelo financeiro)

| Cor | Código (fonte) | Uso |
|---|---|---|
| Azul | `0000FF` | Input ajustável pelo usuário |
| Preto | `000000` | Fórmula / cálculo |
| Verde | `008000` | Link para outra aba |
| Vermelho | `FF0000` | Referência a arquivo externo |
| Fundo amarelo | `FFFF00` | Premissa-chave |

Cada célula de input vai em **azul**; cada célula com `=` vai em **preto**.
Quem abrir a planilha sabe na hora o que pode mexer.

## Aba 1 — Premissas (inputs)

Inputs do usuário (azul), com fundo amarelo nas premissas-chave.

| Célula | Rótulo | Tipo | Formato |
|---|---|---|---|
| B2 | Taxa de desconto (NPV) | input | `0.0%` |
| B3 | Horas economizadas/semana (caso 1) | input | `#,##0` |
| B4 | Custo da hora (R$) | input | `R$ #,##0` |
| B5 | Nº de pessoas impactadas | input | `#,##0` |
| B6 | Aumento de conversêo (%) | input | `0.0%` |
| B7 | Receita base afetada (R$/ano) | input | `R$ #,##0` |
| B8 | Investimento ano 1 (R$) | input | `R$ #,##0` |

## Aba 2 — Investimento (3 anos)

| Categoria | Ano 1 (B) | Ano 2 (C) | Ano 3 (D) | Total (E) |
|---|---|---|---|---|
| Licenças de plataforma de IA | input | input | input | `=SUM(B:D)` da linha |
| Infraestrutura | input | input | input | fórmula |
| Integraçêo | input | input | input | fórmula |
| Serviços / consultoria | input | input | input | fórmula |
| Treinamento & mudança | input | input | input | fórmula |
| Contingência (15%) | `=B*0.15` | fórmula | fórmula | fórmula |
| **Subtotal** | `=SUM(...)` | fórmula | fórmula | fórmula |

> Total de investimento em E: `=SUM(E_linhas)`. Tudo em preto (fórmula), exceto
> os inputs de cada ano em azul.

## Aba 3 — Valor gerado (por ano)

Três blocos somados:

**Ganhos de eficiência**
| Iniciativa | Métrica | Atual | Melhorado | Economia/ano |
|---|---|---|---|---|
| Caso 1 | horas economizadas | input | input | `=Premissas!B3*52*Premissas!B4` |

**Aumento de receita**
| Iniciativa | Métrica | Economia/ano |
|---|---|---|
| Caso 2 | conversêo | `=Premissas!B7*Premissas!B6` |

**Reduçêo de risco**
| Iniciativa | Tipo | Custo evitado |
|---|---|---|
| Caso 3 | compliance | input |

Total de benefícios/ano (preto): `=soma dos três blocos`.

## Aba 4 — Cálculos de ROI

| Métrica | Célula | Fórmula |
|---|---|---|
| ROI simples (%) | B2 | `=(Benefícios_ano1 - Investimento_ano1)/Investimento_ano1` |
| Payback (meses) | B3 | `=Investimento_total/(Benefícios_ano1/12)` |
| Benefício mensal | B4 | `=Benefícios_ano1/12` |

**NPV (3 anos), taxa em `Premissas!B2`:**

| Ano | Benefícios (B) | Custos (C) | Líquido (D) | Fator (E) | VP (F) |
|---|---|---|---|---|---|
| 0 | | input | `=B-C` | `1.00` | `=D*E` |
| 1 | link | link | `=B-C` | `=1/(1+desc)^1` | `=D*E` |
| 2 | link | link | `=B-C` | `=1/(1+desc)^2` | `=D*E` |
| 3 | link | link | `=B-C` | `=1/(1+desc)^3` | `=D*E` |
| **NPV** | | | | | `=SUM(F1:F3)+F0` |

## Aba 5 — Sensibilidade (opcional)

Três cenários (melhor / base / conservador) variando as premissas-chave; cada
cenário recalcula ROI e NPV por fórmula referenciando a aba Premissas.

---

### Lembretes de implementaçêo (openpyxl)
- Indexaçêo **1-based**: `ws.cell(row=1, column=1)` é `A1`.
- Fórmula como string: `ws['E5'] = '=SUM(B5:D5)'`.
- Fonte de input: `Font(color='0000FF')`; fórmula: `Font(color='000000')`.
- Premissa-chave: `PatternFill(start_color='FFFF00', end_color='FFFF00', fill_type='solid')`.
- Formatos: `ws['B4'].number_format = 'R$ #,##0'`; `'0.0%'` para percentuais.
