# Senior Engineering Mentor

Skill (padrão Agent Skills) que transforma o Claude em mentor técnico pessoal para preparação de entrevistas de Software Engineer Sênior: diagnóstico, ensino, entrevistas simuladas, programação, code review, debugging, System Design, análise de currículo/LinkedIn/vaga, inglês e acompanhamento de evolução de longo prazo.

## Estrutura

```
senior-engineering-mentor/
├── SKILL.md                      # Identidade, regras, modos, inicialização, uso do registro
├── SYSTEM_PROMPT.md              # Versão consolidada para outras plataformas
├── README.md
├── references/
│   ├── assessment-rubric.md      # Pontuação, níveis, calibração, pleno vs. sênior, feedback
│   ├── interview-playbook.md     # Entrevistas interativa/completa, follow-ups, comportamental, inglês
│   ├── technical-domains.md      # Domínios e tópicos avaliados (base da matriz)
│   ├── system-design.md          # Metodologia de System Design
│   ├── teaching-methodology.md   # Ensino, revisão, exercícios, adaptação de dificuldade
│   └── progress-tracking.md      # Formato e regras do registro de evolução
├── templates/
│   ├── diagnostic-report.md
│   ├── interview-report.md
│   ├── progress-report.md
│   └── study-plan.md
└── data/
    └── progress-tracking.md      # Registro vivo: perfil, matriz de competências, sessões
```

## Responsabilidade de cada arquivo

| Arquivo | Responsabilidade |
|---|---|
| `SKILL.md` | Núcleo enxuto: metadados, missão, perfil inicial, regras, modos e qual módulo carregar, fluxo de inicialização, regras do registro |
| `references/assessment-rubric.md` | Como avaliar: critérios, pesos, níveis, calibração, pleno vs. sênior |
| `references/interview-playbook.md` | Como conduzir entrevistas e follow-ups |
| `references/technical-domains.md` | O que avaliar e ensinar, por domínio |
| `references/system-design.md` | Como conduzir e avaliar System Design |
| `references/teaching-methodology.md` | Como ensinar, revisar e ajustar dificuldade |
| `references/progress-tracking.md` | Como registrar e atualizar a evolução |
| `templates/*` | Modelos padronizados de relatórios e plano de estudos |
| `data/progress-tracking.md` | Histórico do usuário (separado das instruções) |
| `SYSTEM_PROMPT.md` | Equivalente independente de plataforma |

## Instalação e uso

**Claude (Agent Skills):** copie a pasta para o diretório de skills, por exemplo `~/.claude/skills/senior-engineering-mentor/` (Claude Code) ou envie como skill personalizada no Claude. A skill é ativada automaticamente por pedidos como "me entreviste para sênior", "faça um diagnóstico técnico", "me ensine sobre Kafka", "analise meu currículo".

**Outros agentes:** use `SYSTEM_PROMPT.md` como system prompt (ou instruções de projeto) e mantenha o registro de progresso em um arquivo seu, colando-o no início das sessões.

**Progresso:** quando o agente tem acesso a arquivos, ele atualiza `data/progress-tracking.md`. Sem acesso, ele entrega ao final um bloco pronto para você colar no arquivo e avisa que nada foi salvo. Faça backup do seu `data/progress-tracking.md` antes de atualizar a skill, para não perder o histórico.

## Primeiros passos

1. Diga o que quer: diagnóstico técnico, estudar um assunto, entrevista simulada, exercício ou análise de currículo.
2. Compartilhar currículo/LinkedIn/vaga é opcional.
3. Ao fim de cada sessão, atualize o registro de progresso.
