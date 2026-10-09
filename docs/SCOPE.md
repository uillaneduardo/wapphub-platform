# Escopo do WappHub Platform

**Escopo exclusivo: administração GLOBAL do operador SaaS.** Decisão canônica: [ADR-0001](ADR-0001-M2-ADMIN-BOUNDARIES.md).

## WappHub Admin (uso interno)

- Cadastrar, visualizar, gerenciar e suspender Organizations com auditoria.
- Gerenciar Products, Plans, Features, PlanFeature, Subscription, add-ons e overrides.
- Cadastrar preços, inclusive R$ 0,00, e limites de capacidade.
- Gerenciar assinaturas e faturamento global; acompanhar receita e inadimplência.
- Configurar gateways de pagamento globais (fase específica a detalhar).
- Monitorar diagnósticos e saúde por Organization/Channel/Provider, sem mostrar segredos.
- Consultar consumo agregado de recursos, custos projetados e auditoria administrativa.
- Relatórios globais, indicadores de API/Worker e observabilidade agregada.

## Fora deste frontend

- Minha Conta e administração da própria Organization contratante.
- Configuração operacional de WABA, números, credenciais Meta e webhooks do cliente.
- Atendimento, conversas, contatos, equipes de contratantes.

Essas funções pertencem ao `wapphub-chat`, sob permissão tenant-scoped do Core.

## Segurança

O painel global usa autoridade privilegiada independente de User/Membership de clientes; nenhum OWNER de Organization ganha acesso global. Exigir separação de backend administrativo, autenticação com MFA, isolamento de sessão/credenciais, proteção de rede e auditoria antes da implementação. Controles no frontend nunca substituem autorização no servidor.

## Status

Este documento define escopo futuro, não implementação. Consultar `docs/STATUS.md`. Não alterar o M1 homologado.
