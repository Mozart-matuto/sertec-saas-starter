# SerTec SaaS Starter

Repositório base público para projetos SaaS em .NET com **Web API + Blazor**, pronto para ser clonado e evoluído em produtos (Oráculo, Saúde, etc.) com padrão profissional.

## Objetivo

Entregar uma fundação reutilizável com processo disciplinado:

- Nada de gambiarra.
- Tudo versionado.
- Tudo começa por issue.
- Tudo entra por PR.
- Template manda, projeto obedece.

## Stack alvo

- .NET 8
- ASP.NET Core Web API
- Blazor
- Estrutura para `src/` e `tests/`

## Estrutura do repositório

```text
sertec-saas-starter/
├─ .github/
│  ├─ ISSUE_TEMPLATE/
│  │  ├─ feature.yml
│  │  ├─ bug.yml
│  │  ├─ task.yml
│  │  ├─ tech-debt.yml
│  │  └─ config.yml
│  └─ PULL_REQUEST_TEMPLATE.md
├─ docs/
│  └─ ISSUES_BACKLOG.md
├─ src/
├─ tests/
├─ .editorconfig
├─ Directory.Build.props
├─ global.json
├─ README.md
└─ appsettings.example.json
```

## Fluxo oficial (Issue → Branch → PR)

1. Criar issue usando um template oficial.
2. Criar branch dedicada para a issue.
3. Implementar escopo mínimo necessário.
4. Abrir PR preenchendo template completo.
5. Revisar e fazer merge em `main`.

> Sem issue, não começa. Sem PR com template completo, não entra.

## Tipos de issue

- **Feature**: nova funcionalidade de negócio.
- **Bug**: erro/comportamento incorreto.
- **Task**: tarefa técnica (infra, refatoração, configuração).
- **Tech Debt**: débito técnico assumido conscientemente.

## Branch protection (configuração recomendada)

Configurar proteção em `main` com:

- ✅ Require pull request before merging.
- ✅ Require conversation resolution before merging.
- ⛔ Sem aprovação obrigatória (workflow solo).
- ⛔ Sem CI obrigatório por enquanto.

## Backlog central

Use `docs/ISSUES_BACKLOG.md` como lista mãe.
Cada item do backlog deve virar issue real antes da implementação.

## Uso com Codex + Copilot

- Codex trabalha melhor com issue clara, escopo objetivo e critérios de aceite.
- Fluxo esperado: issue criada → branch da issue → PR da issue.
- Evite tarefas sem contexto: issue bem definida reduz retrabalho.

## Bootstrap

Este starter já inclui:

- templates de issue padronizados;
- template de PR obrigatório;
- backlog central para evolução do SaaS;
- arquivos base de padronização de build/configuração.
