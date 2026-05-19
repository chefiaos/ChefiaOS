# Como usar os cargos

Este documento explica como acionar o time executivo do ChefiaOS no dia a dia.

## Princípio

Todo cargo é um ponto de vista. Cada `ESTRATEGIA_[CARGO].md` ou `CONTEXTO.md` ensina o Claude a pensar daquela perspectiva. Você não precisa decorar a estrutura — o orquestrador `/empresa` escolhe os cargos certos para cada pedido.

## 3 formas de acionar

### 1. Modo automático (mais comum)

Use `/empresa <pedido>` e deixe o orquestrador decidir.

> `/empresa preciso de um carrossel sobre {{tema}}`

O sistema lê a `MATRIZ_COLABORACAO.md`, identifica Social Media Manager + Copywriter + Diretor de Arte + CMO, ativa o protocolo de revisão cruzada e entrega.

### 2. Modo invocação direta

Quando quiser uma perspectiva específica:

> `/empresa quero a visão do CFO sobre aumentar preço em 20%`

O Claude lê `ESTRATEGIA_CFO.md` e responde como CFO.

### 3. Modo mesa redonda

Para temas amplos:

> `/empresa quero uma reunião executiva sobre o próximo trimestre`

Todos os Chiefs apresentam visão. CEO sintetiza. Decisões são registradas em `_decisoes/`.

## Exemplos práticos

| Pedido | Cargos acionados |
|---|---|
| "/empresa rever calendário editorial" | Conteúdo Orgânico + Social Media + CMO |
| "/empresa criar persona da nossa cliente ideal" | Brand Strategist + Copywriter + UX Researcher + CMO |
| "/empresa lançar nova feature de {{X}}" | PM + UX Designer + CPO + CMO + Copywriter + CEO |
| "/empresa nosso churn subiu" | Customer Success + CDO + COO + CPO |
| "/empresa preciso reduzir CAC" | Tráfego Pago + Growth Hacker + CDO + CMO + CFO |
| "/empresa devo contratar agora?" | CHRO + CFO + CEO |

## Quando não usar `/empresa`

- Captura de ideia solta → escreva direto em `_ideias/`.
- Pergunta factual sobre o sistema → leia o arquivo direto.
- Anotação de número/decisão → o registro acontece automaticamente no LOG.
