# MAPA — Onde fica cada coisa

Guia visual da estrutura do ChefiaOS. Para quem não é técnico.

## Raiz

- `README.md` — apresentação pública do sistema.
- `CLAUDE.md` — instruções que o Claude lê antes de responder.
- `MAPA.md` — este arquivo.
- `.gitignore` — arquivos ignorados pelo Git.

## `.claude/commands/`
Skills disponíveis no Claude Code:
- `instalar.md` — configura o sistema na primeira vez.
- `empresa.md` — orquestra os cargos para qualquer tarefa.
- `relatorio.md` — gera relatório executivo mensal.

## `_contexto/`
Coração do sistema. Tudo o que o Claude precisa saber sobre a empresa.
- `CONTEXTO_GERAL.md` — o que é a empresa, público, proposta, modelo.
- `NUMEROS_ATUAIS.md` — métricas atuais (receita, CAC, churn, etc.).

## `identidade/`
- `BRAND.md` — paleta, tom de voz, princípios de copy, frases âncora.

## `templates/`
Estruturas reutilizáveis para conteúdo (10 templates):
- email, roteiro de reel, legenda de instagram, stories, carrossel, persona, calendário editorial, OKR, landing page, script de vendas.

## `_decisoes/`
Memória histórica do negócio.
- `COMO_USAR.md` — explicação do sistema.
- `[ANO]/[MM_mes]/LOG.md` — log mensal de decisões.
- `aprendizados/` — aprendizados atemporais por área.
- `experimentos/` — registros de experimentos rodados.

## `_ideias/`
Brain dump. Ideias soltas, não-validadas. Quando viram decisão, migram para `_decisoes/`.

## Pastas operacionais

- `01_marketing/` — estratégia, conteúdo orgânico, tráfego pago, email, SEO, afiliados.
- `02_vendas/` — funil, pricing, ofertas, parceiros.
- `03_clientes/` — onboarding, suporte, feedback, retenção.
- `04_financeiro/` — receita/custos, métricas SaaS, metas, OKRs.
- `05_produto/` — roadmap, feedback de usuários, experimentos.
- `06_operacoes/` — processos, ferramentas e stack.
- `07_juridico_e_compliance/` — contratos, LGPD, termos.

Cada pasta tem um `GUIA_[AREA].md` que explica o que vai ali.

## `08_estrategia_geral/`

O cérebro estratégico. Contém:
- **8 Chiefs:** CEO, CMO, CFO, CTO, CPO, COO, CDO, CHRO — cada um com seu `ESTRATEGIA_[CARGO].md`.
- **26 funcionários:** distribuídos sob cada Chief, cada um com seu `CONTEXTO.md`.
- **Documentos transversais:**
  - `ORGANOGRAMA.md` — hierarquia visual.
  - `VISAO_E_NORTE.md` — visão, missão, valores.
  - `PAINEL_EXECUTIVO.md` — métricas-chave por Chief.
  - `COMO_USAR_OS_CARGOS.md` — guia prático.
  - `MATRIZ_COLABORACAO.md` — quem faz o quê em cada tipo de tarefa.
  - `PROTOCOLO_REUNIAO_EXECUTIVA.md` — como rodar uma reunião.
  - `PROTOCOLO_REVISAO_CRUZADA.md` — fluxo obrigatório de execução em time.
  - `PROTOCOLO_RESOLUCAO_CONFLITO.md` — quando cargos discordam.
