# Matriz de Colaboração

Tabela que define, para cada tipo de tarefa, quem é **Dono** (executa), **Apoiadores** (opinam antes), e **Aprovador** (valida ao final). Esta é a referência principal usada pela skill `/empresa`.

| # | Tipo de tarefa | Dono | Apoiadores | Aprovador |
|---|---|---|---|---|
| 1 | Criar copy de página/anúncio/email | Copywriter | Brand Strategist, Diretor de Arte | CMO |
| 2 | Definir preço novo / mudar pricing | Pricing Strategist | CFO, Vendas Estrategista | CEO |
| 3 | Lançar feature nova | Product Manager | UX Designer, UX Researcher, CTO, CMO | CPO |
| 4 | Campanha de tráfego pago | Tráfego Pago | Copywriter, Diretor de Arte, CDO | CMO |
| 5 | Investigar churn | Customer Success | CDO, UX Researcher | COO |
| 6 | Criar carrossel | Social Media Manager | Copywriter, Diretor de Arte | CMO |
| 7 | Lead magnet | Copywriter | Growth Hacker, Email Marketing | CMO |
| 8 | Mudança de posicionamento | Brand Strategist | Copywriter, CMO, CEO | CEO |
| 9 | Novo produto / nova linha | Product Manager | CPO, CMO, CFO, CEO | CEO |
| 10 | Contratar alguém | Recrutador Estratégico | Consultor de Cultura, Chief da área | CHRO + CEO |
| 11 | Definir OKRs trimestrais | CEO | Todos os Chiefs | CEO |
| 12 | Reduzir CAC | Tráfego Pago | Growth Hacker, CDO, Copywriter | CMO |
| 13 | Aumentar ativação | UX Designer | Product Manager, Customer Success | CPO |
| 14 | Criar sequência de email | Email Marketing | Copywriter | CMO |
| 15 | Auditoria de SEO | SEO | Copywriter | CMO |
| 16 | Calendário editorial | Conteúdo Orgânico | Social Media Manager, Copywriter | CMO |
| 17 | Construir persona | Brand Strategist | UX Researcher, Copywriter | CMO |
| 18 | Programa de afiliados | Parcerias & Afiliados | CMO, CFO | COO |
| 19 | Mudar fluxo de onboarding | UX Designer | Customer Success, Product Manager | CPO |
| 20 | Definir estrutura organizacional | CHRO | CEO, Chief afetado | CEO |
| 21 | Adotar nova ferramenta | Processos | CTO, CFO, Chief que vai usar | COO |
| 22 | Reagir a queda de receita | CEO | CFO, CMO, CPO, COO | CEO |
| 23 | Criar dashboard executivo | Analista de BI | Chief solicitante | CDO |
| 24 | Rodar experimento de growth | Analista de Experimentos | Growth Hacker, área impactada | CDO |
| 25 | Plano de retenção / win-back | Customer Success | Email Marketing, Copywriter | COO |
| 26 | Definir oferta / pacote comercial | Vendas Estrategista | Pricing Strategist, CFO, Copywriter | CEO |
| 27 | Roteiro de reel | Copywriter | Social Media Manager, Diretor de Arte | CMO |
| 28 | Script de vendas | Vendas Estrategista | Copywriter | CEO |
| 29 | Adequação LGPD | Processos | CTO, CEO | COO |
| 30 | Revisão semanal / planejamento | CEO | Chiefs relevantes | CEO |
| 31 | Ritual interno / cultural | Consultor de Cultura | CHRO, CEO | CHRO |
| 32 | Análise de unit economics | Analista Financeiro | CFO, CDO | CFO |
| 33 | Programa de comunidade | Gestor de Comunidade | Community Manager, CMO | COO |
| 34 | Reescrita técnica / refatoração | CTO | Product Owner | CTO |

## Como ler

- **Dono executa.** Faz o trabalho, escreve, decide o miúdo.
- **Apoiadores opinam ANTES do dono executar.** Cada um em sua especialidade.
- **Aprovador valida ao final.** Tem 3 respostas possíveis: "aprovado", "mudar X", "refazer".

Se a tarefa não estiver listada aqui, o orquestrador `/empresa` usa a matriz de roteamento por palavras-chave em `commands/empresa.md` ou pede ajuda ao CEO para definir.
