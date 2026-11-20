# Agente Shopfire — Segurança Contra Incêndio (SP)

Assistente técnico-comercial da Shopfire para **regularização de AVCB/CLCB, projetos técnicos e adequação de edificações**, baseado no **Decreto Estadual nº 69.118/2024** e nas **Instruções Técnicas (ITs) do CBPMESP – edição 2025**.

> ⚠️ O agente é ferramenta de apoio. Toda decisão técnica é do responsável técnico (engenheiro/arquiteto com ART/RRT).

---

## Estrutura do repositório

```
shopfire-agente/
├── README.md                ← este arquivo
├── CLAUDE.md                ← regras e comportamento do agente
├── PREENCHER/               ← ✍️ VOCÊ PREENCHE (o diferencial da empresa)
│   ├── 01-empresa.md
│   ├── 02-servicos-e-precos.md
│   ├── 03-clientes-vencimentos.csv
│   ├── 04-comunique-se-historico.md
│   ├── 05-projetos-modelo.md
│   └── 06-equipe-e-responsaveis.md
├── normas/                  ← textos oficiais convertidos em .md
│   ├── INDICE.md            ← lista de ITs + status de atualização
│   ├── decreto-69118-2024.md   (colocar)
│   └── its/                 ← uma IT por arquivo (colocar)
├── fluxos/                  ← "funções" do agente, passo a passo
│   ├── 01-enquadramento.md
│   ├── 02-checklist-vistoria.md
│   ├── 03-pre-analise-projeto.md
│   ├── 04-resposta-comunique-se.md
│   ├── 05-plano-adequacao.md
│   ├── 06-proposta-comercial.md
│   └── 07-controle-renovacoes.md
└── modelos/
    ├── proposta-comercial.md
    └── relatorio-vistoria.md
```

---

## Passo a passo para colocar no ar

### 1. Preencher a pasta `PREENCHER/`
Comece por `01-empresa.md` e `02-servicos-e-precos.md`. São ~30 minutos e já deixam o agente útil.

### 2. Colocar as normas em `normas/`
1. Baixe as ITs e o Decreto 69.118/2024 em **www.corpodebombeiros.sp.gov.br**.
2. Converta cada PDF para Markdown (pode pedir ao Claude: "converta este PDF da IT 11 em markdown mantendo a numeração dos itens e as tabelas").
3. Salve como `normas/its/IT-11-saidas-de-emergencia.md` etc.
4. Atualize a coluna de status em `normas/INDICE.md`.

### 3. Subir no GitHub
```bash
git init
git add .
git commit -m "Agente Shopfire - estrutura inicial"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/shopfire-agente.git
git push -u origin main
```
➡️ Deixe o repositório **privado** (tem preços e dados de clientes).

### 4. Usar o agente — escolha um modo

| Modo | Para quem | Como |
|---|---|---|
| **Projeto no Claude** (simples) | Equipe toda, pelo celular/PC | Crie um Projeto "Shopfire", cole o `CLAUDE.md` nas instruções e envie os arquivos de `normas/`, `PREENCHER/`, `fluxos/` e `modelos/`. Ou conecte o repositório do GitHub ao Projeto. |
| **Claude Code** (avançado) | Quem faz projeto e revisão | Abra o repositório no Claude Code. Ele lê o `CLAUDE.md` automaticamente e consegue revisar memoriais, gerar propostas e atualizar planilhas dentro do repo. |

### 5. Manutenção mensal (15 min)
- Verificar portarias novas do CCB no Diário Oficial e consultas públicas.
- Substituir as ITs alteradas e registrar em `normas/INDICE.md`.
- Acrescentar os Comunique-se do mês em `04-comunique-se-historico.md`.
- Atualizar vencimentos em `03-clientes-vencimentos.csv`.

---

## Exemplos de pedidos para o agente
- "Enquadra: restaurante, 480 m², térreo, com cozinha a GLP. CLCB ou AVCB? Quais sistemas?"
- "Gera o checklist de vistoria para um galpão de depósito de 2.500 m²."
- "Recebi esse Comunique-se [colar texto]. Como respondo?"
- "Prédio residencial de 1985, 8 andares, sem AVCB. Monta o plano de adequação."
- "Faz a proposta comercial para o enquadramento acima."
- "Quais clientes vencem nos próximos 90 dias?"
