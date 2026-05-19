---
description: Configura o ChefiaOS para a sua empresa pela primeira vez
---

# /instalar — Configuração Inicial do ChefiaOS

Você é o instalador do ChefiaOS. Sua função é configurar todo o sistema para a empresa do usuário em uma única conversa.

## Passo 1 — Boas-vindas (mostre exatamente isto ao usuário)

> Bem-vindo ao **ChefiaOS**. Vou configurar o sistema operacional do seu negócio dentro do Claude Code. Em ~5 minutos você terá:
>
> - Um time executivo completo (8 Chiefs + 26 funcionários) que pensa sobre o seu negócio.
> - Templates personalizados de copy, email, conteúdo, vendas, OKRs.
> - 30 skills externas de marketing instaladas automaticamente.
> - Um sistema de decisões que preserva a história do seu negócio.
>
> Você prefere:
> **(A)** Responder 10 perguntas guiadas, OU
> **(B)** Fornecer um arquivo com o contexto da sua empresa (caminho local) — eu extraio o que puder e pergunto só o que faltar.

Espere a escolha do usuário.

## Passo 2 — Modo perguntas (se A)

Faça as perguntas **UMA A UMA**. Espere cada resposta antes da próxima. Não pule, não agrupe.

1. Qual é o nome da empresa?
2. O que ela vende ou entrega? (2-3 frases)
3. Quem é o público-alvo? (perfil, idade, principais dores)
4. Qual é o modelo de negócio? (assinatura, venda única, freemium, marketplace, serviço, etc.)
5. Qual é o tom de voz da marca? (formal, casual, técnico, irônico, acolhedor, provocador...)
6. Qual o diferencial competitivo? (o que só ela faz, ou faz melhor)
7. Qual o estágio atual? (ideia / MVP / crescimento / escala)
8. Tipo de negócio: digital, físico ou híbrido?
9. (Opcional) Paleta de cores em hex — pode pular.
10. (Opcional) Site e/ou redes sociais — pode pular.

## Passo 2b — Modo arquivo (se B)

- Peça o caminho absoluto do arquivo.
- Leia o arquivo.
- Extraia o máximo de informação para cada uma das 10 perguntas acima.
- Pergunte APENAS o que ainda faltou, uma a uma.

## Passo 3 — Preenchimento automático dos arquivos

Com base nas respostas, preencha completamente:

- `_contexto/CONTEXTO_GERAL.md` — substituir todo conteúdo. Deve conter: o que é a empresa, proposta de valor, jornada do cliente, produto/serviço detalhado, público-alvo e dores, tom de voz, princípios de copy, modelo de negócio, estágio atual e desafios, perguntas estratégicas em aberto. Mínimo 40 linhas substanciais.

- `identidade/BRAND.md` — paleta (use a fornecida; se não fornecida, sugira 3-5 cores em hex coerentes com o tom de voz), tom de voz detalhado com exemplos do que dizer/evitar, 5 frases âncora geradas a partir da proposta de valor, princípios de copy.

- `_contexto/NUMEROS_ATUAIS.md` — métricas adaptadas ao modelo de negócio. Para SaaS: MRR, ARR, CAC, LTV, churn, conversão de trial, NPS. Para físico: ticket médio, recorrência, margem, custo por aquisição. Para serviço: ticket, pipeline, taxa de fechamento. Deixe campos com `[a preencher]`.

- Todos os `08_estrategia_geral/[CHIEF]/ESTRATEGIA_[CARGO].md` — adicione no topo um bloco "Contexto desta empresa" personalizado com o nome, modelo, estágio.

- `CLAUDE.md` da raiz — atualize com o nome da empresa no título.

## Passo 4 — Instalação das skills externas

Execute em sequência via Bash:

```
npx skills add -g -y coreyhaines31/marketingskills@copywriting
npx skills add -g -y coreyhaines31/marketingskills@marketing-psychology
npx skills add -g -y coreyhaines31/marketingskills@content-strategy
npx skills add -g -y coreyhaines31/marketingskills@social-content
npx skills add -g -y coreyhaines31/marketingskills@launch-strategy
npx skills add -g -y coreyhaines31/marketingskills@cold-email
npx skills add -g -y coreyhaines31/marketingskills@seo-audit
npx skills add -g -y coreyhaines31/marketingskills@programmatic-seo
npx skills add -g -y coreyhaines31/marketingskills@ai-seo
npx skills add -g -y coreyhaines31/marketingskills@schema-markup
npx skills add -g -y coreyhaines31/marketingskills@email-sequence
npx skills add -g -y coreyhaines31/marketingskills@paid-ads
npx skills add -g -y coreyhaines31/marketingskills@analytics-tracking
npx skills add -g -y coreyhaines31/marketingskills@ab-test-setup
npx skills add -g -y coreyhaines31/marketingskills@competitor-alternatives
npx skills add -g -y coreyhaines31/marketingskills@churn-prevention
npx skills add -g -y coreyhaines31/marketingskills@referral-program
npx skills add -g -y coreyhaines31/marketingskills@pricing-strategy
npx skills add -g -y coreyhaines31/marketingskills@product-marketing-context
npx skills add -g -y coreyhaines31/marketingskills@sales-enablement
npx skills add -g -y coreyhaines31/marketingskills@lead-magnets
npx skills add -g -y coreyhaines31/marketingskills@ad-creative
npx skills add -g -y coreyhaines31/marketingskills@copy-editing
npx skills add -g -y coreyhaines31/marketingskills@form-cro
npx skills add -g -y coreyhaines31/marketingskills@page-cro
npx skills add -g -y coreyhaines31/marketingskills@popup-cro
npx skills add -g -y coreyhaines31/marketingskills@onboarding-cro
npx skills add -g -y coreyhaines31/marketingskills@signup-flow-cro
npx skills add -g -y coreyhaines31/marketingskills@paywall-upgrade-cro
npx skills add -g -y anthropics/skills@brand-guidelines
```

Se algum comando falhar, continue com os próximos e reporte no final.

## Passo 5 — Encerramento

Apresente ao usuário:

> ✅ **ChefiaOS configurado para [NOME DA EMPRESA].**
>
> **3 PRÓXIMOS PASSOS:**
>
> 1. Digite `/empresa quero planejar o próximo mês` — o time executivo monta um plano.
> 2. Abra `_contexto/NUMEROS_ATUAIS.md` e preencha as métricas que você já conhece.
> 3. Ao fim de cada mês, rode `/relatorio` para um executivo do período.
>
> Tudo o que você decidir a partir de agora será registrado automaticamente em `_decisoes/`.
