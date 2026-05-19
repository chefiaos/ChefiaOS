# ChefiaOS — Documento Completo

## O que é

ChefiaOS é um sistema operacional de negócio instalado dentro do Claude Code. Ele transforma o Claude em um time executivo completo da sua empresa — com memória persistente, identidade de marca centralizada, protocolos de colaboração entre cargos e registro automático de decisões.

Não é um chatbot. É uma infraestrutura estratégica que vive junto com o seu negócio, aprende com ele e cresce com ele.

---

## Como funciona

Após a instalação, o Claude passa a conhecer profundamente a sua empresa: quem você é, o que vende, para quem, como se comunica, quais são seus números e quais decisões já foram tomadas. Cada vez que você pede algo, ele aciona os especialistas certos para entregar a melhor resposta.

**Tudo funciona por um único comando:**
```
/empresa [o que você quer fazer]
```

O sistema identifica o tipo de tarefa, consulta a matriz de colaboração, aciona os cargos relevantes, aplica o protocolo de revisão cruzada e entrega o resultado final.

---

## Os 3 comandos

### `/instalar`
Configura o sistema pela primeira vez. Faz perguntas sobre o negócio (ou lê um arquivo de contexto pronto) e preenche automaticamente:
- Contexto geral da empresa
- Identidade visual e tom de voz
- Painel de métricas personalizado ao modelo de negócio
- Todos os 36 arquivos de cargo com a lente do seu negócio
- Instala 30 skills externas especializadas

### `/empresa`
O comando universal. Interpreta qualquer pedido e aciona os cargos certos. Exemplos do que entende:

| O que você digita | O que acontece |
|-------------------|----------------|
| `/empresa quero criar um carrossel sobre X` | Social Media + Copywriter + Diretor de Arte + aprovação do CMO |
| `/empresa meu churn aumentou` | Customer Success + CDO + COO |
| `/empresa qual preço cobrar pelo novo produto` | Pricing Strategist + CFO + CEO |
| `/empresa preciso de um email de reativação` | Gestor de Email + Copywriter + Customer Success + CMO |
| `/empresa quero planejar o próximo trimestre` | CEO + todos os Chiefs |
| `/empresa reunião geral sobre crescimento` | Mesa redonda com 8 Chiefs |
| `/empresa criar campanha de tráfego pago` | Gestor de Tráfego + Copywriter + Diretor de Arte + CMO + CFO |
| `/empresa montar lead magnet` | Copywriter + Growth Hacker + CMO |
| `/empresa atualizar contexto da empresa` | Re-executa partes do /instalar |
| `/empresa anotar uma ideia` | Captura em `_ideias/` |
| `/empresa revisar a semana` | CEO + Chiefs principais |
| `/empresa persona do cliente` | Brand Strategist + Copywriter + CMO |
| `/empresa calendário editorial do mês` | Gestor de Conteúdo + Social Media + CMO |

### `/relatorio`
Gera relatório executivo mensal lendo automaticamente os números atuais e o histórico de decisões do período. Entrega:
- Resumo executivo (3 bullets: bom, ruim, muda)
- Números do período comparados ao mês anterior
- Decisões tomadas
- Status dos experimentos ativos
- O que funcionou e o que não funcionou
- 3 prioridades para os próximos 30 dias

---

## O Time — 8 Chiefs + 28 Funcionários

### CEO — Chief Executive Officer
Visão geral, estratégia, crescimento e decisões de alto nível. Quebra empates entre Chiefs. Define norte e prioridades.

**Funcionários:**
- Vendas Estrategista — scripts, funil, fechamento
- Consultor de Pricing & Vendas — precificação estratégica

---

### CMO — Chief Marketing Officer
Marketing, aquisição, conteúdo, copy e marca.

**Funcionários:**
- **Copywriter** — textos de venda, landing pages, emails, anúncios
- **Gestor de Conteúdo Orgânico** — estratégia e produção de conteúdo
- **Gestor de Tráfego Pago** — Meta Ads, Google Ads, campanhas
- **Especialista em SEO** — orgânico, técnico, programático
- **Community Manager** — resposta a comentários, engajamento, comunidade
- **Gestor de Email Marketing** — sequências, newsletters, automações
- **Brand Strategist** — identidade, posicionamento, tom de voz
- **Social Media Manager** — estratégia e operação das redes sociais
- **Diretor de Arte** — identidade visual, criativos, peças

---

### CFO — Chief Financial Officer
Financeiro, métricas, custos, pricing e metas.

**Funcionários:**
- **Analista Financeiro** — receita, custos, margens, fluxo de caixa
- **Pricing Strategist** — estratégia de preço, testes, posicionamento

---

### CTO — Chief Technology Officer
Tecnologia, dados, infraestrutura e growth.

**Funcionários:**
- **Growth Hacker** — experimentos de crescimento, funil, otimização
- **Analista de Dados** — métricas, dashboards, análise de comportamento

---

### CPO — Chief Product Officer
Produto, experiência do usuário e roadmap.

**Funcionários:**
- **Product Manager** — roadmap, priorização, discovery
- **Product Owner** — backlog, sprint, entrega
- **UX Designer** — interface, fluxos, usabilidade
- **UX Researcher** — pesquisa com usuários, validação

---

### COO — Chief Operating Officer
Operações, processos, clientes e parcerias.

**Funcionários:**
- **Customer Success** — ativação, retenção, sucesso do cliente
- **Suporte ao Cliente** — atendimento, FAQ, resolução de problemas
- **Gestor de Parcerias & Afiliados** — programa de afiliados, co-marketing
- **Gestor de Processos** — SOPs, automações, eficiência operacional
- **Gestor de Comunidade** — grupos, memberships, comunidade paga

---

### CDO — Chief Data Officer
Dados, analytics, experimentos e decisões baseadas em evidências.

**Funcionários:**
- **Analista de Experimentos** — A/B tests, hipóteses, validações
- **Analista de BI** — relatórios, visualizações, insights estratégicos

---

### CHRO — Chief Human Resources Officer
Pessoas, cultura e time.

**Funcionários:**
- **Consultor de Cultura** — valores, ambiente, rituais de time
- **Recrutador Estratégico** — perfis, processos seletivos, onboarding

---

## Protocolos de colaboração

### Matriz de Colaboração
Para cada tipo de tarefa, define quem é o **Dono**, os **Apoiadores** e o **Aprovador final**. São 34 tipos de tarefa mapeados. Garante que nenhuma entrega passe por apenas uma perspectiva.

### Protocolo de Revisão Cruzada
Fluxo obrigatório antes de qualquer entrega:
1. Apoiadores opinam em ordem de relevância
2. Dono executa considerando os inputs
3. Aprovador valida ou pede ajuste
4. Hand-off explícito com resumo do processo

### Protocolo de Resolução de Conflito
Quando dois Chiefs discordam, o CEO decide com base em: visão de longo prazo, estágio atual da empresa e métricas reais. Decisão registrada automaticamente no log.

### Protocolo de Reunião Executiva
Mesa redonda com todos os Chiefs: cada um apresenta sua visão → identificam consenso e conflito → propõem decisões → CEO fecha. Output registrado em `_decisoes/`.

---

## Sistema de memória e decisões

Toda decisão, resultado, aprendizado ou número mencionado é registrado automaticamente em `_decisoes/[ANO]/[MM_mes]/LOG.md`.

**Três tipos de registro:**
- **Log mensal** — decisões e resultados do mês
- **Aprendizados atemporais** — o que vale para sempre (por área: Marketing, Financeiro, Produto, Clientes, Operações)
- **Experimentos** — hipótese, métrica de sucesso, resultado, aprendizado

Quando você pergunta "o que ficou decidido sobre X?", o Claude busca no log antes de responder.

---

## 30 skills externas instaladas automaticamente

| Skill | Cargo que potencializa |
|-------|----------------------|
| `copywriting` | Copywriter |
| `marketing-psychology` | Brand Strategist |
| `content-strategy` | Gestor de Conteúdo |
| `social-content` | Social Media Manager |
| `launch-strategy` | CEO + CMO |
| `cold-email` | Copywriter + Vendas |
| `seo-audit` | SEO Specialist |
| `programmatic-seo` | SEO Specialist |
| `ai-seo` | SEO Specialist |
| `schema-markup` | SEO Specialist |
| `email-sequence` | Gestor de Email |
| `paid-ads` | Gestor de Tráfego |
| `analytics-tracking` | Analista de Dados |
| `ab-test-setup` | Analista de Experimentos |
| `competitor-alternatives` | CDO + CEO |
| `churn-prevention` | Customer Success |
| `referral-program` | COO + CMO |
| `pricing-strategy` | Pricing Strategist |
| `product-marketing-context` | Product Manager |
| `sales-enablement` | Vendas Estrategista |
| `lead-magnets` | Copywriter + Growth Hacker |
| `ad-creative` | Diretor de Arte |
| `copy-editing` | Copywriter |
| `form-cro` | Growth Hacker + UX |
| `page-cro` | Growth Hacker + UX |
| `popup-cro` | Growth Hacker |
| `onboarding-cro` | Customer Success + UX |
| `signup-flow-cro` | Growth Hacker + UX |
| `paywall-upgrade-cro` | Growth Hacker + CFO |
| `brand-guidelines` | Brand Strategist |

---

## 10 templates prontos

Estruturas reutilizáveis que o Claude usa automaticamente ao gerar conteúdo:

- **Email** — boas-vindas, reativação, promoção
- **Roteiro de Reel** — gancho, desenvolvimento, virada, CTA
- **Legenda Instagram** — carrossel, reel, quote
- **Stories** — sequência de campanha completa
- **Carrossel** — 9 slides com função por slide
- **Persona** — demográfico, psicográfico, dores, gatilhos
- **Calendário Editorial** — tabela 30 dias por pilar
- **OKR** — objetivo + key results por cargo
- **Landing Page** — estrutura de seções completa
- **Script de Vendas** — abertura, descoberta, fechamento

---

## Estrutura de pastas gerada

```
SeuNegocio/
├── _contexto/
│   ├── CONTEXTO_GERAL.md     Tudo sobre a empresa
│   └── NUMEROS_ATUAIS.md     Métricas vivas
├── identidade/
│   └── BRAND.md              Paleta, tipografia, tom de voz, frases âncora
├── templates/                10 templates operacionais
├── _decisoes/
│   ├── 2025/01_janeiro/LOG.md
│   ├── aprendizados/         Por área
│   └── experimentos/
├── _ideias/                  Brain dump de ideias não-validadas
├── 01_marketing/
├── 02_vendas/
├── 03_clientes/
├── 04_financeiro/
├── 05_produto/
├── 06_operacoes/
├── 07_juridico_e_compliance/
└── 08_estrategia_geral/      C-Suite + 28 funcionários + protocolos
```

---

## Para quem é

- **Founders solos** que precisam pensar em todas as áreas mas não têm time
- **Pequenas empresas** que querem operar com nível de empresa maior
- **Agências** que precisam de visão estratégica para os clientes
- **Qualquer negócio** — digital, físico ou híbrido

---

## Pré-requisitos

- VS Code ou qualquer editor com terminal integrado
- Git
- Node.js (LTS)
- Claude Code (`npm install -g @anthropic-ai/claude-code`) com plano Pro

---

## Instalação

Crie uma pasta com o nome do seu negócio, abra no Claude Code e cole:

```
Clona o https://github.com/caiocarvalhar/ChefiaOS na pasta atual, entra nela e roda o /instalar.
```

Em ~5 minutos seu time executivo está operacional.
