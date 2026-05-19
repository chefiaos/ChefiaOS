# Instruções para o Claude — ChefiaOS

Este arquivo orienta como o Claude deve operar dentro deste sistema. Leia antes de qualquer resposta.

## Detecção de primeiro uso

Se o arquivo `_contexto/CONTEXTO_GERAL.md` ainda contém o marcador `⚠️ Vazio`, isso significa que o sistema nunca foi configurado. **Rode `/instalar` automaticamente** antes de qualquer outra resposta.

## Leituras obrigatórias antes de responder

1. **Sempre:** `_contexto/CONTEXTO_GERAL.md` — para entender o negócio.
2. **Antes de criar conteúdo (copy, post, email, roteiro):** `identidade/BRAND.md` — para tom de voz, paleta, princípios.
3. **Antes de gerar email, roteiro, legenda, carrossel, story, landing, script de vendas:** o template correspondente em `templates/`.
4. **Para perguntas sobre métricas, receita, CAC, churn, etc:** `_contexto/NUMEROS_ATUAIS.md`.
5. **Para invocar um cargo específico:** o `CONTEXTO.md` correspondente em `08_estrategia_geral/`.

## Sistema de cargos

Existem 8 Chiefs e 26 funcionários em `08_estrategia_geral/`. Quando o usuário pedir a visão de um cargo, leia o respectivo `ESTRATEGIA_[CARGO].md` (Chief) ou `CONTEXTO.md` (funcionário) antes de responder.

Para qualquer ação coletiva (envolvendo mais de um cargo), use:
- `08_estrategia_geral/MATRIZ_COLABORACAO.md` — identifica Dono, Apoiadores, Aprovador.
- `08_estrategia_geral/PROTOCOLO_REVISAO_CRUZADA.md` — fluxo obrigatório de execução.
- `08_estrategia_geral/PROTOCOLO_RESOLUCAO_CONFLITO.md` — quando dois cargos discordam.

---

## REGRA PRINCIPAL — Registro automático de decisões

**Toda vez que o usuário tomar uma decisão, relatar um resultado, mencionar algo que funcionou ou não, citar um número (receita, CAC, conversão, churn) ou indicar uma mudança de direção — você DEVE registrar automaticamente em `_decisoes/[ANO]/[MM_mes]/LOG.md`.**

### O que salvar
- Decisões estratégicas ("vou focar em orgânico antes de ads")
- Resultados de experimentos
- O que funcionou e o que não funcionou
- Insights de usuários
- Mudanças de direção
- Números relevantes com a data

### Onde salvar
1. **Sempre:** `_decisoes/[ANO]/[MM_mes]/LOG.md` (crie a pasta se não existir).
2. **Se for aprendizado atemporal:** salve também em `_decisoes/aprendizados/[AREA].md`.
3. **Se for um experimento:** salve em `_decisoes/experimentos/[NOME].md`.

### Formato obrigatório de cada entrada

```
## [DATA] — [TÍTULO]
**Tipo:** Decisão / Resultado / Aprendizado / Experimento
**Área:** Marketing / Vendas / Produto / Financeiro / Operações / Clientes
**Cargo relevante:** CEO / CMO / CFO / CTO / CPO / COO / CDO / CHRO

**O que aconteceu / foi decidido:**
[descrição objetiva]

**Por quê:**
[motivação ou contexto]

**Resultado (se já souber):**
[preencher quando souber]

**Aprendizado:**
[o que isso ensina]

**Próximo passo:**
[ação concreta]
```

---

## Outras instruções

- Quando criar conteúdo aprovado (copy, roteiro, email), sugira salvar na pasta operacional correspondente.
- Quando o usuário perguntar "o que ficou decidido sobre X?", busque em `_decisoes/` antes de responder.
- **Nunca apague entradas antigas do log** — a história é o ativo mais valioso.
- Se houver ambiguidade sobre o que o usuário quer, pergunte antes de executar.
- Para qualquer tarefa que envolva múltiplas perspectivas, use `/empresa` como orquestrador.
