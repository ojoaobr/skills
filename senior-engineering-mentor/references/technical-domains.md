# Technical Domains

Mapa de competências avaliadas. Os nomes dos domínios abaixo são os mesmos usados na matriz de `data/progress-tracking.md`. Amplie o escopo sempre que identificar conhecimento relevante para sênior.

## Domínios técnicos

### 1. Linguagens e fundamentos de programação
Modelos de execução, memória (stack/heap), tipos, paradigmas (OO, funcional), imutabilidade, tratamento de erros, complexidade, fundamentos de computação (SO, redes, I/O).

### 2. C# e .NET
CLR, GC (gerações, LOH, pressão de memória), async/await e state machine, Task vs. thread, `Span<T>`/alocação, LINQ e execução diferida, DI e ciclo de vida, ASP.NET Core (pipeline, middleware), EF Core (tracking, N+1, queries), HttpClientFactory, configuração, diagnóstico (dotnet-counters, traces).

### 3. Estruturas de dados e algoritmos
Arrays, listas, hash maps, heaps, árvores, grafos, tries; ordenação, busca, two pointers, sliding window, DP, backtracking, greedy; análise de complexidade e escolha de estrutura por padrão de acesso.

### 4. Arquitetura de software
Clean Architecture, hexagonal, DDD (bounded contexts, agregados, eventos de domínio), monólito modular vs. microsserviços, acoplamento/coesão, ADRs, evolução arquitetural.

### 5. Design Patterns e SOLID
Criacionais, estruturais, comportamentais; quando aplicar e quando é over-engineering; SOLID com exemplos de violação reais; patterns de resiliência e integração (Outbox, Saga, CQRS, Strangler Fig, Anti-Corruption Layer).

### 6. Bancos de dados
SQL, índices (B-tree, cobertura, seletividade), plano de execução, transações e níveis de isolamento, locks e deadlocks, modelagem, normalização vs. desnormalização; NoSQL (MongoDB: modelagem de documentos, índices, sharding, consistência), escolha relacional vs. não relacional, replicação e particionamento.

### 7. APIs e protocolos
HTTP/1.1, 2, 3, TLS, REST (maturidade, idempotência, versionamento, paginação), SOAP/WSDL, gRPC, GraphQL, contratos e compatibilidade, rate limiting, autenticação e autorização (OAuth2, OIDC, JWT).

### 8. Microsserviços
Fronteiras de serviço, comunicação síncrona vs. assíncrona, dados por serviço, versionamento de contratos, migração incremental de monólito, API gateway, service discovery, custos operacionais.

### 9. Sistemas distribuídos
CAP/PACELC, modelos de consistência, relógios e ordenação, consenso (conceitos de Raft/Paxos), replicação, particionamento, falhas parciais, idempotência, exactly-once vs. at-least-once, transações distribuídas (Saga, 2PC), timeouts, retries, circuit breaker, backpressure.

### 10. Mensageria
RabbitMQ (exchanges, filas, acks, DLQ, prefetch), Kafka (partições, offsets, consumer groups, retenção, compaction, rebalance, ordering, entrega), outbox/inbox, deduplicação, poison messages, esquemas e evolução de eventos, escolha de broker.

### 11. Concorrência e paralelismo
Threads, locks, memory model, race conditions, deadlock, async I/O vs. paralelismo de CPU, `Channel<T>`, `SemaphoreSlim`, estruturas concorrentes, Interlocked, cancelamento, filas e pipelines produtor-consumidor.

### 12. Performance e escalabilidade
Profiling (CPU, memória, I/O), gargalos, caching (aside, write-through, invalidação, stampede), CDN, escala horizontal/vertical, balanceamento, redução de alocações e consumo de CPU/memória, testes de carga, filas para absorver picos.

### 13. System Design
Metodologia em `system-design.md`: requisitos, estimativas, modelagem, componentes, escalabilidade, falhas, trade-offs.

### 14. Cloud Computing
Modelos IaaS/PaaS/serverless, redes (VPC, subnets), identidade e permissões, storage, filas gerenciadas, bancos gerenciados, custos, multi-AZ/região, princípios de well-architected (AWS/Azure/GCP).

### 15. Docker e Kubernetes
Imagens e camadas, boas práticas de Dockerfile, rede e volumes; Pods, Deployments, Services, Ingress, probes, requests/limits, HPA, ConfigMap/Secret, rolling update, troubleshooting.

### 16. CI/CD e DevOps
Pipelines, estratégias de branch, trunk-based, deploy (blue/green, canary, feature flags), rollback, IaC (Terraform/Bicep), gestão de segredos, DORA metrics.

### 17. Testes automatizados
Pirâmide, unitário, integração, contrato, E2E, TDD, mocks vs. fakes, testes de concorrência e de resiliência, testabilidade do design, flakiness, cobertura vs. qualidade.

### 18. Segurança
OWASP Top 10, autenticação/autorização, gestão de segredos, criptografia (conceitos), validação de entrada, injeção, SSRF, supply chain, princípio do menor privilégio, segurança em mensageria e APIs.

### 19. Observabilidade
Logs estruturados, métricas, traces distribuídos, correlação, OpenTelemetry, SLI/SLO/SLA, alertas acionáveis, dashboards, investigação de incidentes, postmortems.

### 20. Inteligência Artificial aplicada à engenharia
Uso de assistentes de código com revisão crítica, limites e riscos (alucinação, segurança, licenciamento), engenharia de prompts, integração de LLMs em produto (RAG, custos, latência, avaliação), impacto no fluxo de desenvolvimento.

### 21. Comunicação técnica
Explicar com clareza para públicos distintos, documentação, RFCs e ADRs, argumentação de decisões, escrita de design docs.

### 22. Inglês profissional
Vocabulário técnico, clareza e fluência em entrevistas, escrita técnica, apresentação de experiências e decisões em inglês.

### 23. Liderança e tomada de decisão
Decisão com incerteza, priorização, mentoria, code review como ferramenta de ensino, influência sem autoridade, gestão de dívida técnica, comunicação com stakeholders, ownership e resposta a incidentes.

## Como usar

- Diagnóstico: percorra os domínios em ordem de relevância para a meta do usuário, 2–4 perguntas por domínio, partindo do fundamental.
- Trilha: priorize domínios com lacuna crítica e alta relevância para entrevistas sênior (System Design, sistemas distribuídos, mensageria, concorrência, bancos, algoritmos).
- Domínios não avaliados permanecem "Não avaliado" na matriz.
