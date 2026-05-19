---
description: Gera um relatório executivo mensal do negócio
---

# /relatorio — Relatório Executivo Mensal

Você gera um relatório executivo do mês corrente (ou do mês indicado pelo usuário).

## Passo 1 — Definir o período

Se o usuário não especificou, use o mês atual. Pergunte se quiser confirmar.

## Passo 2 — Coletar fontes

Leia, na ordem:
1. `_contexto/NUMEROS_ATUAIS.md` — métricas atuais.
2. `_decisoes/[ANO]/[MM_mes]/LOG.md` — todas as decisões do mês.
3. `_decisoes/experimentos/*.md` — experimentos com resultado no mês.
4. `_contexto/CONTEXTO_GERAL.md` — contexto base.
5. `08_estrategia_geral/PAINEL_EXECUTIVO.md` — referência de painel.

## Passo 3 — Estrutura obrigatória do relatório

```
# Relatório Executivo — [MÊS]/[ANO]

## 1. Resumo Executivo
3-5 frases. O que aconteceu de mais relevante. Tom executivo.

## 2. Números do mês
Tabela ou lista com métricas-chave e variação vs mês anterior.

## 3. Decisões tomadas
Lista das decisões registradas no LOG do mês, com 1 linha de contexto cada.

## 4. Experimentos
Quais rodaram, métrica, resultado, conclusão.

## 5. O que funcionou
3-5 itens com evidência.

## 6. O que não funcionou
3-5 itens com hipótese do porquê.

## 7. Próximos 30 dias
3-5 prioridades concretas, com cargo responsável.
```

## Passo 4 — Salvar

Salve o relatório em `_decisoes/[ANO]/[MM_mes]/RELATORIO_MES.md`. Se já existir, sobrescreva após confirmar.

## Passo 5 — Apresentar

Mostre o relatório completo ao usuário no chat, depois informe o caminho onde foi salvo.
