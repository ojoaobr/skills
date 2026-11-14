# Progress Tracking

Regras e formato do registro de evolução. O registro em si fica em `data/progress-tracking.md`, separado das instruções.

## 1. Princípios

- Instruções permanentes (este diretório `references/`) e histórico (`data/`) nunca se misturam.
- Registre informação relevante para acompanhar evolução; não transcreva conversas inteiras.
- Só registre o que foi observado ou informado pelo usuário. Nunca invente fatos, métricas ou notas.
- "Não avaliado" ≠ "desconhecido".
- Nunca afirme que algo foi salvo se a escrita não ocorreu.

## 2. Estrutura de `data/progress-tracking.md`

1. **Perfil profissional** — informações fornecidas pelo usuário ou extraídas de currículo/LinkedIn, marcando "comprovada" vs. "mencionada".
2. **Metas** — cargo-alvo, empresas, prazo, idioma da entrevista.
3. **Matriz de competências** — uma linha por domínio (mesmos nomes de `technical-domains.md`): estado, nota atual, evidências, pontos fortes, lacunas, última avaliação, próxima revisão.
4. **Histórico de sessões** — uma entrada por sessão (mais recente primeiro).
5. **Dificuldades recorrentes.**
6. **Próximas prioridades.**

## 3. Matriz de competências

Estados permitidos: **Não avaliado, Básico, Intermediário, Avançado, Domínio consistente**.

Regras de atualização:

- Estado inicial de todo domínio: Não avaliado.
- Atualize a nota atual como média ponderada recente (as últimas 3 avaliações, com mais peso para as mais novas); registre a data.
- Mude o estado só com pelo menos 3 evidências em contextos distintos; antes disso, anote "(provisório)".
- Rebaixe o estado apenas com evidência nova contrária e consistente.
- Próxima revisão: Básico em ~1 semana; Intermediário em ~2–3 semanas; Avançado em ~1–2 meses; Domínio consistente em ~3 meses.
- Evidências: referencie a sessão (data) e o tipo (pergunta, exercício, entrevista).

## 4. Entrada de sessão (formato)

```
### AAAA-MM-DD — <tema da sessão>
- Modo: <diagnóstico | ensino | entrevista | programação | system design | análise | inglês | revisão>
- Assuntos: ...
- Perguntas/exercícios: ... (notas)
- Respostas relevantes: ... (apenas o que ajuda a evoluir)
- Competências demonstradas: ...
- Dificuldades: ...
- Recomendações: ...
- Atualizações na matriz: <domínio: estado/nota>
- Próximos passos: ...
```

## 5. Quando atualizar

- Ao final de cada sessão com avaliação, ensino relevante ou exercício concluído.
- Após análise profissional (seção de perfil).
- Após entrevistas simuladas (inclua link/nome do relatório gerado).
- Não atualize por conversas triviais.

## 6. Como atualizar

**Com acesso a arquivos:** leia o arquivo atual, edite apenas as seções afetadas (matriz, histórico, prioridades), confirme que a escrita foi concluída e informe ao usuário o que mudou.

**Sem acesso a arquivos:** gere um bloco "Atualização de progresso" com a entrada de sessão e as linhas da matriz alteradas, pronto para colar no arquivo, e avise que **nada foi salvo automaticamente**. No início de uma nova sessão, peça ao usuário para colar o conteúdo do registro, se ele quiser continuar de onde parou.

## 7. Privacidade

Armazene só o necessário para a evolução. Não registre dados sensíveis desnecessários (documentos de identificação, informações financeiras, dados pessoais de terceiros).

## 8. Continuidade

No início de uma sessão: leia o registro, resuma em 2–3 linhas o ponto atual e as prioridades, e pergunte se o usuário quer seguir a trilha ou escolher outro assunto.
