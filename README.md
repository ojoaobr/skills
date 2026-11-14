# Skills

Coleção de skills no padrão [Agent Skills](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) para o Claude. Cada pasta é uma skill independente, com seu próprio `SKILL.md` e um `README.md` com detalhes de estrutura e uso.

## Skills disponíveis

| Skill | Descrição |
|---|---|
| [senior-engineering-mentor](senior-engineering-mentor/) | Mentor técnico pessoal para preparação de entrevistas de Software Engineer Sênior: diagnóstico, ensino, entrevistas simuladas, desafios de programação, code review, debugging, System Design, análise de currículo/LinkedIn/vaga, inglês e acompanhamento de evolução de longo prazo. |

### senior-engineering-mentor

Transforma o Claude em um mentor que combina Staff Engineer, Tech Lead, entrevistador e professor. O foco é desenvolver competências reais, não só decorar respostas de entrevista.

- **Modos:** diagnóstico técnico, ensino de um assunto, entrevista simulada (técnica, System Design, comportamental), exercícios, code review e análise de currículo.
- **Progresso:** mantém um registro de evolução em `data/progress-tracking.md`, com perfil, matriz de competências e histórico de sessões.
- **Ativação:** pedidos como "me entreviste para sênior", "faça um diagnóstico técnico", "me ensine sobre Kafka" ou "analise meu currículo".
- **Outras plataformas:** `SYSTEM_PROMPT.md` traz uma versão consolidada para usar como system prompt em qualquer agente.

Mais detalhes em [senior-engineering-mentor/README.md](senior-engineering-mentor/README.md).

## Instalação

**Claude Code:** copie a pasta da skill para `~/.claude/skills/` (skills pessoais) ou para `.claude/skills/` dentro de um projeto:

```bash
git clone https://github.com/ojoaobr/skills.git
cp -r skills/senior-engineering-mentor ~/.claude/skills/
```

**Claude.ai:** compacte a pasta da skill em um `.zip` e envie como skill personalizada.

A skill é carregada automaticamente quando o pedido combina com a `description` do `SKILL.md`.

## Estrutura do repositório

```
skills/
├── README.md
└── senior-engineering-mentor/
    ├── SKILL.md          # Metadados e instruções principais
    ├── SYSTEM_PROMPT.md  # Versão independente de plataforma
    ├── README.md
    ├── references/       # Módulos carregados sob demanda
    ├── templates/        # Modelos de relatórios e plano de estudos
    └── data/             # Registro de progresso do usuário
```

## Adicionando uma nova skill

1. Crie uma pasta com o nome da skill (kebab-case).
2. Adicione um `SKILL.md` com frontmatter `name` e `description`.
3. Inclua um `README.md` explicando estrutura e uso.
4. Adicione uma linha na tabela de [Skills disponíveis](#skills-disponíveis).
