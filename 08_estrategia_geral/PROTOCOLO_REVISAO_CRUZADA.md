# Protocolo de Revisão Cruzada

Fluxo **obrigatório** sempre que `/empresa` ativa mais de um cargo. Garante que toda entrega final passe por múltiplas perspectivas antes de chegar ao usuário.

## Por que existe

Sem este protocolo, o Claude tende a executar a tarefa sozinho e devolver um resultado raso. Com ele, cada cargo contribui no seu ponto forte e o aprovador catches problemas que o dono não viu.

## Fluxo (4 passos)

### Passo 1 — Apoiadores opinam
Cada apoiador, em ordem de relevância para a tarefa, escreve **3-6 linhas** com sua leitura. Não executa nada ainda. Apenas:
- Aponta riscos ou oportunidades específicas.
- Sinaliza informações faltantes.
- Sugere ângulo ou abordagem.

### Passo 2 — Dono executa
O dono lê todas as opiniões dos apoiadores e produz a entrega. Pode discordar de um apoiador, mas precisa justificar por que escolheu não seguir aquela sugestão.

### Passo 3 — Aprovador valida
O aprovador lê a entrega e responde **uma das três**:
- **Aprovado** — segue para o usuário.
- **Mudar X** — pede ajuste pontual; o dono ajusta e segue.
- **Refazer** — algo central está errado; volta ao passo 1 com nova orientação.

### Passo 4 — Hand-off e entrega final
- Se houver dependência entre cargos (ex: Copywriter precisa do briefing do Brand Strategist), o hand-off é explícito: "Brand Strategist entrega X → Copywriter recebe X e produz Y".
- A entrega ao usuário inclui:
  - O conteúdo principal (o que ele pediu).
  - **Resumo curto do processo:** quem opinou, qual foi a decisão central, o que foi descartado.

## Exemplo aplicado — "criar carrossel"

1. **Apoiadores opinam:**
   - Copywriter: "promessa precisa ser específica, sugiro ângulo X"
   - Diretor de Arte: "considerar contraste no slide 1, hierarquia tipográfica"
2. **Dono (Social Media Manager) executa:** monta os 9 slides usando o template, incorporando as sugestões.
3. **Aprovador (CMO) valida:** aprovado / mudar slide 7 / refazer.
4. **Entrega:** carrossel completo + 3 linhas dizendo "Copywriter sugeriu ângulo X. Diretor de Arte ajustou hierarquia no slide 1. CMO aprovou."

## Quando pular o protocolo

Apenas em duas situações:
1. Tarefa com **um único cargo** envolvido (anotação simples, captura de ideia).
2. **Urgência declarada pelo usuário** — registrar no LOG que a revisão cruzada foi pulada.
