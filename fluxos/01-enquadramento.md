# Fluxo 01 — Enquadramento Rápido

**Objetivo:** dizer em minutos se o caso é **CLCB, PTS ou PT/AVCB** e **quais sistemas são exigidos**.

## 1. Coletar dados (perguntar o que faltar)
| Dado | Exemplo |
|---|---|
| Uso / atividade | restaurante, depósito, escola, condomínio |
| Área construída total (m²) | 480 |
| Altura (m) / nº de pavimentos | térreo / 2 pav. |
| Subsolo? | sim/não, uso |
| Lotação estimada | 120 pessoas |
| GLP ou gás natural? | P-45, 2 cilindros |
| Materiais armazenados / carga de incêndio | |
| Edificação nova ou existente? Ano? Já teve AVCB? | |
| Endereço / município | |

## 2. Classificar
1. **Ocupação/divisão** → tabela de classificação do Decreto 69.118/2024.
2. **Altura** → tipo conforme a tabela de altura do Decreto.
3. **Carga de incêndio** → IT 14 (risco baixo/médio/alto).

## 3. Definir o tipo de licenciamento
Conferir na IT 01 e IT 42 os critérios de **CLCB**, **PTS** e **PT**. Citar o item exato.

## 4. Listar exigências
Usar a tabela de exigências do Decreto para a divisão + área + altura. Para cada sistema, apontar a IT de referência.

## 5. Saída (formato)
```
ENQUADRAMENTO — [nome/uso]
Classificação: [divisão] — [Decreto, Tabela X]
Altura: [tipo] | Carga de incêndio: [MJ/m² — risco]
Licenciamento: [CLCB / PTS / PT] — [IT 01/42, item X]

Sistemas exigidos:
| Sistema | Exigido? | IT de referência | Observação |
|---|---|---|---|
| Extintores | ✅ | IT 21 | |
| Sinalização | ✅ | IT 20 | |
| ... | | | |

Documentos/laudos prováveis: [ ]
Pontos de atenção: [ ]
Próximo passo sugerido: [proposta / visita técnica]
⚠️ Validar com o responsável técnico antes de protocolar.
```
