# Fluxo 02 — Checklist de Vistoria

**Objetivo:** gerar checklist para a **pré-vistoria da Shopfire** (antes do Bombeiro ir) de acordo com os sistemas exigidos no enquadramento.

## Entrada
Resultado do Fluxo 01 (ou dados da edificação).

## Montagem
Para cada sistema exigido, puxar os requisitos verificáveis em campo da IT correspondente, sempre com o item.

## Blocos padrão (ajustar ao caso)
- **Documentos no local:** licença anterior, ARTs/RRTs, atestados (brigada, elétrico, GLP, CMAR), projeto aprovado.
- **Extintores (IT 21):** tipo/capacidade, distribuição, altura de fixação, validade, sinalização, desobstrução.
- **Sinalização (IT 20):** rotas de fuga, saídas, equipamentos, proibição/alerta, fotoluminescência.
- **Iluminação (IT 18):** autonomia, pontos de rota, teste de funcionamento.
- **Saídas de emergência (IT 11):** larguras, portas (sentido, barra antipânico quando exigida), corrimãos/guarda-corpos, desobstrução.
- **Alarme/detecção (IT 19):** acionadores, avisadores, central, teste.
- **Hidrantes (IT 22):** abrigo, mangueiras, esguicho, reserva técnica, bomba, teste de pressão.
- **GLP (IT 28):** central/abrigo, afastamentos, ventilação, laudo de estanqueidade.
- **Brigada (IT 17):** quantidade, certificados válidos.
- **CMAR (IT 10):** materiais de acabamento, laudos/atestados.
- **Elétrica (IT 41):** inspeção visual, laudo.

## Saída (formato)
Tabela por ambiente/sistema:
| # | Item a verificar | IT / item | OK | Não conforme | N/A | Foto | Observação |
|---|---|---|---|---|---|---|---|

Final: lista de não conformidades → vira orçamento de adequação (Fluxo 06).
Use o modelo `modelos/relatorio-vistoria.md`.
