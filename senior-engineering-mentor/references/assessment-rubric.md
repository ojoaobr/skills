# Assessment Rubric

Critérios para avaliar respostas, exercícios e entrevistas. Toda nota deve citar evidências observadas.

## 1. Pontuação (0 a 10)

| Critério | Peso | O que observar |
|---|---:|---|
| Precisão técnica | 25% | Fatos corretos, terminologia adequada, ausência de erros conceituais |
| Profundidade | 20% | Funcionamento interno, casos de borda, "por quê" além do "o quê" |
| Aplicabilidade prática | 20% | Uso em produção, exemplos reais, problemas operacionais conhecidos |
| Argumentação e trade-offs | 20% | Alternativas comparadas, decisão justificada, limites reconhecidos |
| Clareza na comunicação | 15% | Estrutura, concisão, adaptação ao interlocutor |

Nota final = soma ponderada das notas por critério (cada uma de 0 a 10), com uma casa decimal.

## 2. Classificação

| Nota | Nível |
|---|---|
| 0–3,9 | Insuficiente |
| 4–5,9 | Básico |
| 6–7,4 | Intermediário |
| 7,5–8,4 | Avançado |
| 8,5–9,4 | Domínio consistente |
| 9,5–10 | Excelência |

Para a matriz de competências, "Excelência" é registrada como "Domínio consistente" (os estados da matriz são: Não avaliado, Básico, Intermediário, Avançado, Domínio consistente). "Insuficiente" é registrada como "Básico" com lacuna crítica anotada.

## 3. Regras de calibração

- Definição correta e nada além: no máximo 5,9 (Básico).
- Nota 7,5 ou mais exige aplicação prática e trade-offs, não só teoria.
- Nota 8,5 ou mais exige funcionamento interno, falhas em produção e alternativas, de forma consistente.
- Teoria sem capacidade de aplicar é diferente de prática sem teoria; registre ambas separadamente quando divergirem.
- Uma nota isolada nunca define o nível da competência. Estime o nível por pelo menos 3 evidências em contextos distintos; antes disso, marque a estimativa como "provisória".
- Respostas decoradas: sinais são vocabulário correto com falha ao receber um cenário novo, incapacidade de explicar o "por quê", exemplos genéricos. Teste com follow-up em cenário de produção.
- Seja consistente: o mesmo nível de resposta recebe a mesma nota em sessões diferentes.

## 4. Pleno vs. sênior

| Dimensão | Pleno | Sênior |
|---|---|---|
| Problema | Resolve o problema dado | Questiona e reformula o problema; levanta requisitos e restrições |
| Soluções | Uma solução funcional | Várias alternativas com trade-offs e critério de escolha |
| Escopo | Componente ou serviço | Sistema, múltiplos times, evolução ao longo do tempo |
| Falhas | Trata erros previstos | Antecipa modos de falha, degradação, recuperação, idempotência |
| Produção | Faz funcionar | Observabilidade, operação, custo, segurança, rollout seguro |
| Profundidade | Sabe usar a tecnologia | Explica funcionamento interno e quando não usar |
| Decisão | Segue padrões | Decide com incerteza, documenta, assume consequências |
| Comunicação | Explica o que fez | Convence, alinha stakeholders, adapta o nível de detalhe |
| Liderança | Executa bem | Influencia, orienta outros, eleva a qualidade do time |

Em todo feedback, aponte explicitamente o que faltou para a resposta sair do patamar pleno e chegar ao sênior.

## 5. Estrutura do feedback

1. Nota (com notas por critério quando útil).
2. Acertos.
3. Erros e omissões.
4. O que precisa ser aprofundado.
5. Perguntas complementares (antes de revelar a resposta, quando pedagogicamente adequado).
6. Resposta de referência.
7. Diferença entre pleno e sênior neste tema.

## 6. Avaliação por tipo de atividade

**Programação:** correção, complexidade de tempo/espaço, legibilidade, tratamento de erros e casos de borda, testabilidade, decisões de implementação.

**Code review/debugging:** bugs encontrados vs. existentes, priorização por severidade, qualidade da explicação da causa raiz, sugestão de correção e de teste.

**System Design:** ver `system-design.md` (rubrica por etapa).

**Comportamental:** estrutura (contexto, responsabilidade, ação, resultado), especificidade, ownership, aprendizado, ausência de métricas inventadas.

**Inglês:** avalie separadamente conteúdo técnico e linguagem (vocabulário, clareza, fluência, organização, argumentação). A nota técnica não deve ser penalizada por erros gramaticais que não prejudicam o entendimento.

## 7. Prontidão simulada

Quando solicitada, estime a prontidão para uma posição sênior com base apenas nas evidências registradas: competências avaliadas vs. não avaliadas, consistência das notas, lacunas críticas. Declare o nível de confiança e deixe claro que é uma estimativa, não garantia de aprovação em processos seletivos.
