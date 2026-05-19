# ChefiaOS

**Sistema operacional de negócio para Claude Code.** Instalável em qualquer empresa em menos de 5 minutos.

ChefiaOS transforma o Claude Code em um time executivo completo: 8 Chiefs (C-Suite) + 26 funcionários especializados, todos com perspectivas próprias, métricas e protocolos de colaboração. É a infraestrutura de pensamento estratégico de uma empresa, materializada em arquivos de markdown que o Claude lê antes de cada resposta.

---

## Instalação

### Pré-requisitos (instale uma vez, na ordem)

**1. VS Code**
Baixe em [code.visualstudio.com](https://code.visualstudio.com). Instale com as opções padrão.

**2. Git**
Baixe em [git-scm.com/downloads](https://git-scm.com/downloads). Instale com as opções padrão. No Mac já vem instalado.

**3. Node.js**
Baixe a versão **LTS** em [nodejs.org](https://nodejs.org). Instale com as opções padrão.

**4. Claude Code**
Abra o terminal (Prompt de Comando no Windows, Terminal no Mac) e cole:
```
npm install -g @anthropic-ai/claude-code
```
Depois digite `claude` e faça login com sua conta Anthropic (necessário plano Pro).

---

### Instalando o ChefiaOS

**Caminho fácil (recomendado)**

1. Crie uma pasta no seu computador com o nome do seu negócio (ex: `MeuNegocio`)
2. Abra ela no VS Code (Arquivo → Abrir Pasta)
3. Abra o terminal integrado (`Ctrl+'` no Windows / `Cmd+'` no Mac)
4. Digite `claude` e dê Enter
5. Cole esse prompt:

```
Clona o https://github.com/caiocarvalhar/ChefiaOS na pasta atual, entra nela e roda o /instalar.
```

**Caminho pelo terminal**
```bash
git clone https://github.com/caiocarvalhar/ChefiaOS.git .
```
Abra a pasta no VS Code, abra o terminal integrado, digite `claude` e depois `/instalar`.

---

### O que acontece durante o `/instalar`

A skill faz perguntas sobre o seu negócio (ou aceita um arquivo de contexto pronto), preenche todos os documentos do sistema automaticamente e instala as 30 skills externas necessárias. Em ~5 minutos seu time executivo está pronto.

**Pronto.** Use `/empresa <pedido>` para qualquer tarefa do negócio.

---

## 3 skills principais

- `/instalar` — Configuração inicial do sistema para a sua empresa.
- `/empresa` — Orquestra os cargos para qualquer tarefa do negócio.
- `/relatorio` — Gera relatório executivo mensal.

---

## C-Suite (8 Chiefs)

CEO, CMO, CFO, CTO, CPO, COO, CDO, CHRO.

## Funcionários (26 cargos)

- **CEO:** Vendas Estrategista, Pricing & Vendas
- **CMO:** Copywriter, Conteúdo Orgânico, Tráfego Pago, SEO, Community Manager, Email Marketing, Brand Strategist, Social Media Manager, Diretor de Arte
- **CFO:** Analista Financeiro, Pricing Strategist
- **CTO:** Growth Hacker, Analista de Dados
- **CPO:** Product Manager, Product Owner, UX Designer, UX Researcher
- **COO:** Customer Success, Suporte, Parcerias & Afiliados, Processos, Gestor de Comunidade
- **CDO:** Analista de Experimentos, Analista de BI
- **CHRO:** Consultor de Cultura, Recrutador Estratégico

---

## 30 skills externas instaladas automaticamente

Pacote `coreyhaines31/marketingskills` (29 skills): copywriting, marketing-psychology, content-strategy, social-content, launch-strategy, cold-email, seo-audit, programmatic-seo, ai-seo, schema-markup, email-sequence, paid-ads, analytics-tracking, ab-test-setup, competitor-alternatives, churn-prevention, referral-program, pricing-strategy, product-marketing-context, sales-enablement, lead-magnets, ad-creative, copy-editing, form-cro, page-cro, popup-cro, onboarding-cro, signup-flow-cro, paywall-upgrade-cro. Mais `anthropics/skills@brand-guidelines`.

---

## Sistema de decisões

Toda decisão, resultado, aprendizado ou número relevante mencionado pelo usuário é registrado automaticamente em `_decisoes/[ANO]/[MM_mes]/LOG.md`. Aprendizados atemporais vão para `_decisoes/aprendizados/`. Experimentos vão para `_decisoes/experimentos/`. Esse log é o ativo mais valioso do sistema: ele preserva a história e permite que o Claude responda perguntas como "o que ficou decidido sobre X?".

---

## Estrutura de pastas

```
ChefiaOS/
├── _contexto/            Contexto geral da empresa e números atuais
├── identidade/           Brand, paleta, tom de voz
├── templates/            10 templates operacionais (email, reel, carrossel, etc.)
├── _decisoes/            Log histórico de decisões, aprendizados, experimentos
├── _ideias/              Brain dump de ideias não-validadas
├── 01_marketing/         Estratégia, conteúdo, tráfego, email, SEO, afiliados
├── 02_vendas/            Funil, pricing, ofertas, parceiros
├── 03_clientes/          Onboarding, suporte, feedback, retenção
├── 04_financeiro/        Receita, métricas SaaS, metas, OKRs
├── 05_produto/           Roadmap, feedback, experimentos
├── 06_operacoes/         Processos, ferramentas
├── 07_juridico_e_compliance/
└── 08_estrategia_geral/  C-Suite + 26 funcionários + protocolos
```
