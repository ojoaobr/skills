# Interview Playbook

Procedimentos para entrevistas simuladas de nível sênior. Notas e níveis: `assessment-rubric.md`. Relatório final: `templates/interview-report.md`.

## 1. Preparação

Antes de começar, defina com o usuário (poucas perguntas, em uma mensagem):

- Tipo: técnica geral, algoritmos, System Design, comportamental, mista, por tecnologia.
- Formato: interativa ou completa.
- Idioma: português ou inglês.
- Empresa/vaga alvo, se houver (ajuste o estilo: Big Tech, produto, consultoria).
- Duração ou quantidade de perguntas (padrão: 45–60 minutos, 5–8 perguntas).

## 2. Entrevista interativa

- Uma pergunta por vez; aguarde a resposta.
- Comece com pergunta aberta; aprofunde com follow-ups sobre o que o usuário disse.
- Questione decisões e pressupostos ("por que essa escolha?", "o que acontece se...?").
- Não entregue dicas prematuramente. Se o usuário travar, dê uma pista mínima e registre que houve ajuda.
- Aumente a dificuldade quando a resposta for sólida; simplifique o ângulo (não o conteúdo) quando houver dificuldade.
- Ao final de cada pergunta, dê o feedback no formato da seção 5 do `assessment-rubric.md`.

## 3. Entrevista completa

- Simule uma entrevista real: apresente-se como entrevistador, estabeleça duração e número de perguntas, conduza sem interrupções.
- **Não dê feedback, nota nem dica durante a simulação.** Follow-ups são permitidos como um entrevistador real faria, sem sinalizar acerto ou erro.
- Ao encerrar, avalie com `templates/interview-report.md`: nota geral, notas por competência, respostas satisfatórias e insuficientes, exemplos de respostas melhores, recomendação simulada (aprovação ou não aprovação) com a ressalva de que é uma estimativa.
- Se o usuário pedir para parar no meio, encerre e avalie o que foi feito.

## 4. Banco de follow-ups

Use para testar compreensão real:

- Funcionamento interno: "o que acontece por baixo quando...?"
- Falha: "o que acontece se esse componente cair/atrasar/duplicar mensagem?"
- Escala: "e com 100x mais carga? onde quebra primeiro?"
- Alternativa: "por que não X? quando X seria melhor?"
- Consistência: "como garante que isso não executa duas vezes?"
- Produção: "como você detectaria esse problema? que métrica/alerta?"
- Custo e operação: "qual o custo operacional dessa escolha?"
- Evolução: "como migraria isso sem downtime?"
- Cenário novo: mude uma restrição e veja se o raciocínio se adapta.

## 5. Perguntas comportamentais

Foque em liderança técnica e decisão: conflito técnico, decisão sob incerteza, falha em produção, mentoria, influência sem autoridade, priorização, discordância com o time, dívida técnica, migração de monólito.

- Estruture com o usuário: contexto, responsabilidade, ação/decisões e justificativas, resultado, aprendizado.
- Use experiências reais do usuário; peça detalhes quando faltar contexto.
- **Nunca invente métricas, resultados ou responsabilidades.** Se o usuário não tem o número, ajude a descrever o impacto qualitativamente.
- Avalie: especificidade, ownership ("eu" vs. "nós"), pensamento sistêmico, autocrítica.

## 6. Entrevistas em inglês

Avalie **separadamente**:

- Conhecimento técnico (mesma rubrica).
- Linguagem: vocabulário técnico, clareza, fluência, organização do raciocínio, capacidade de argumentação.

Durante entrevista completa, não corrija; ao final, apresente correções gramaticais e versões mais naturais e profissionais das respostas, mantendo o foco técnico. Em modo interativo, corrija apenas erros que prejudiquem o entendimento e deixe o restante para o feedback.

## 7. Encerramento

1. Entregue feedback/relatório conforme o formato.
2. Liste 2–3 prioridades de estudo.
3. Atualize o registro de progresso (`references/progress-tracking.md`): perguntas, notas, evidências, dificuldades.
