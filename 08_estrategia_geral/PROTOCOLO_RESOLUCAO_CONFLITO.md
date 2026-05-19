# Protocolo de Resolução de Conflito

Usado quando dois ou mais cargos discordam **fundamentalmente** sobre uma decisão e a discussão não converge naturalmente.

## Quando acionar

- Quando o desacordo não é sobre execução, mas sobre **direção**.
- Quando ambos os lados têm argumento legítimo dentro da própria perspectiva.
- Quando o impasse trava a entrega para o usuário.

## Quem decide

O **CEO** sempre. Conflito não se resolve por maioria, se resolve por hierarquia + critério.

## Fluxo (5 passos)

### 1. Ouvir os dois lados
Cada cargo em conflito apresenta sua posição em **4-6 linhas**:
- O que defende
- Por que defende
- Qual o risco de fazer o contrário

### 2. Identificar o trade-off central
O CEO nomeia explicitamente o trade-off em uma frase. Exemplos:
- "Margem de curto prazo vs aquisição agressiva."
- "Qualidade técnica vs velocidade de feature."
- "Foco em base atual vs expansão de público."

Se não conseguir nomear o trade-off, o conflito é falso (geralmente é falta de informação).

### 3. Consultar as três fontes de critério
O CEO decide com base em, nesta ordem:
1. **`VISAO_E_NORTE.md`** — qual decisão preserva melhor a visão de longo prazo?
2. **`_contexto/CONTEXTO_GERAL.md`** — qual decisão faz sentido para o estágio atual?
3. **`_contexto/NUMEROS_ATUAIS.md`** — qual decisão a realidade financeira aguenta?

### 4. Decidir e justificar
Decisão em 1 frase + justificativa em 2-4 linhas conectando às fontes acima. Sem ambiguidade.

### 5. Registrar
Entrada obrigatória em `_decisoes/[ANO]/[MM_mes]/LOG.md` com:
- Tipo: Decisão
- O conflito original
- Os dois lados
- O trade-off nomeado
- A decisão
- O critério usado
- O que será observado para validar a decisão

## Princípio

Conflito bem resolvido é ativo, não problema. Ele força clareza. Mas conflito que se repete é sintoma de que falta uma decisão estrutural ainda não tomada — sinalizar no LOG para revisão futura.
