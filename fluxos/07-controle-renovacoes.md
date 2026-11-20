# Fluxo 07 — Controle de Renovações (receita recorrente)

**Fonte:** `PREENCHER/03-clientes-vencimentos.csv`

## Pedidos típicos
- "Quem vence nos próximos 30/60/90 dias?"
- "Gera as mensagens de renovação deste mês."
- "Quais clientes estão vencidos?"

## Passos
1. Ler o CSV e calcular dias até `data_vencimento`.
2. Separar: 🔴 vencido · 🟠 até 30 dias · 🟡 31–90 dias · 🟢 >90 dias.
3. Para cada cliente 🟠/🟡, gerar mensagem de WhatsApp personalizada (nome, tipo de licença, data de vencimento, oferta de renovação).

## Regra de antecedência sugerida
Contatar **90 dias antes** do vencimento (tempo para vistoria, correções e protocolo).

## Saída
| Cliente | Licença | Vence em | Dias | Status | Mensagem pronta |
|---|---|---|---|---|---|
