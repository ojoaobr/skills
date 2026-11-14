# System Design

Metodologia para entrevistas e treino de arquitetura em nível sênior. Notas: `assessment-rubric.md`.

## 1. Condução da sessão

- Apresente um problema realista e deliberadamente vago (ex.: "projete um encurtador de URLs", "pipeline de processamento de eventos de alto volume", "sistema de notificações", "migração de monólito de pagamentos"). Prefira, quando possível, problemas ligados à experiência do usuário (mensageria, alto volume, migração de monólito).
- Não entregue a solução. Deixe o usuário conduzir; faça perguntas e introduza cenários de falha e mudanças de requisito.
- Duração típica: 45–60 min. Ofereça modo interativo (com intervenções) ou completo (feedback só ao final).

## 2. Etapas e o que avaliar

| # | Etapa | Evidência esperada de nível sênior |
|---|---|---|
| 1 | Requisitos | Faz perguntas de escopo; separa funcionais e não funcionais (latência, disponibilidade, consistência, durabilidade, custo, conformidade); define o que fica de fora |
| 2 | Estimativas | Usuários, QPS médio e de pico, volume de dados, banda, retenção; ordens de grandeza corretas e premissas explícitas |
| 3 | API e modelo de dados | Contratos claros, idempotência, paginação, versionamento; modelagem guiada pelos padrões de acesso; escolha do banco justificada |
| 4 | Arquitetura de alto nível | Componentes mínimos necessários, responsabilidades claras, fluxo de dados de ponta a ponta |
| 5 | Aprofundamento | Escolhe 1–2 componentes críticos e os detalha (particionamento, índices, filas, cache, algoritmos) |
| 6 | Escalabilidade | Identifica o gargalo, escala horizontal, sharding, cache, filas, backpressure, hot keys |
| 7 | Consistência e disponibilidade | Escolhas explícitas (CAP/PACELC), modelo de consistência por caso de uso, idempotência, deduplicação, ordenação |
| 8 | Falhas e resiliência | Timeouts, retries com backoff e jitter, circuit breaker, DLQ, degradação graciosa, recuperação de desastres, rollout seguro |
| 9 | Segurança | Autenticação/autorização, proteção de dados, limites de abuso, segredos |
| 10 | Observabilidade e operação | Métricas/SLOs, logs, traces, alertas, runbooks, capacidade |
| 11 | Custos e trade-offs | Compara alternativas, explicita o que se sacrifica, evolução em fases |

## 3. Perguntas de provocação

- "Qual é o primeiro componente a quebrar com 10x de carga?"
- "O que acontece se esta fila/partição/zona ficar indisponível por 30 minutos?"
- "Como evitar processar o mesmo evento duas vezes? E perder um?"
- "Como garante ordenação onde ela importa?"
- "Como migraria dos dados atuais para este desenho sem downtime?"
- "Por que não usar [alternativa mais simples]? Esse desenho não é over-engineering?"
- "Como saberia, em produção, que isto está degradando?"
- "Qual o custo aproximado e onde é possível economizar?"

## 4. Armadilhas comuns

Começar a desenhar sem requisitos; pular estimativas; adicionar tecnologias sem necessidade; ignorar falhas; consistência "mágica"; cache sem estratégia de invalidação; microsserviços sem justificativa; não discutir trade-offs; ignorar operação e custo.

## 5. Avaliação

Notas de 0 a 10 por etapa (ou agrupadas) com a rubrica geral. Em sênior, pesa mais: condução do processo, trade-offs explícitos, tratamento de falhas e capacidade de priorizar. Entregue ao final: pontos fortes, lacunas, desenho de referência resumido, e a diferença entre uma resposta de pleno e de sênior neste problema.

## 6. Roteiro de estudo

Fundamentos (latência, throughput, estimativas) → blocos (cache, filas, bancos, balanceadores, CDN) → padrões (sharding, replicação, outbox, saga, CQRS, event sourcing, rate limiting) → casos clássicos (encurtador de URL, feed, chat, notificações, pipeline de eventos, busca, armazenamento de arquivos, pagamentos) → mock interviews cronometradas.
