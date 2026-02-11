# Backlog central do SerTec SaaS Starter

Este documento é a **lista-mãe** da fundação SaaS.
Cada item deve ser convertido em issue (`Feature`, `Bug`, `Task` ou `Tech Debt`) antes de implementação.

## Autenticação

- [ ] Login com JWT
- [ ] Controle de roles/perfis
- [ ] Lockout e rate limiting
- [ ] Auditoria de autenticação
- [ ] Proteção de endpoints administrativos

## Licenças

- [ ] Entidade de licença por tenant
- [ ] Regras de trial inicial
- [ ] Controle de seats máximos
- [ ] Bloqueio por expiração
- [ ] Fluxo de ativação e revogação

## Multi-tenant

- [ ] Entidade Tenant
- [ ] TenantId obrigatório no contexto
- [ ] Isolamento de dados por tenant
- [ ] Testes anti-vazamento entre tenants
- [ ] Administração de tenants

## Infraestrutura

- [ ] Estrutura inicial da solução (`src/` e `tests/`)
- [ ] Docker Compose de desenvolvimento
- [ ] Configuração de ambientes
- [ ] Estratégia de migrações
- [ ] Versionamento semântico e convenções de release

## Observabilidade

- [ ] Logging estruturado
- [ ] Correlação por request/tenant
- [ ] Métricas de saúde da aplicação
- [ ] Tracing distribuído (quando aplicável)
- [ ] Alertas mínimos operacionais

## Segurança

- [ ] Políticas de segredo e configuração segura
- [ ] Validação e sanitização de entrada
- [ ] Hardening de autenticação/autorização
- [ ] Auditoria de eventos críticos
- [ ] Revisão de dependências e vulnerabilidades

## UI base (Blazor)

- [ ] Layout base de aplicação
- [ ] Tela de login
- [ ] Shell administrativo inicial
- [ ] Componentes reutilizáveis de formulário
- [ ] Página padrão de erro e estados vazios
