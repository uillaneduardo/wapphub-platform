# WappHub Platform

Frontend de administração GLOBAL e privilegiada do ecossistema WappHub. **Não é portal de contratantes.**

## Escopo global

- Organizações/clientes do SaaS, planos, produtos, recursos e preços (inclusive R$ 0,00).
- Assinaturas, assentos, overrides e intervenções administrativas auditáveis.
- Faturamento global, relatórios, inadimplência e configuração dos gateways de pagamento (por milestones específicos).
- Diagnóstico global das integrações e consumo, monitoramento técnico e auditoria privilegiada.

## Fronteira de confiança

Autenticação administrativa independente, MFA, APIs privilegiadas protegidas, isolamento de sessão/credenciais/permissões em relação ao Chat. Ser OWNER de uma Organization não concede privilégio global.

**Gestão de equipe, Meta, consumo, assinatura e faturamento da própria Organization pertence ao [wapphub-chat](https://github.com/uillaneduardo/wapphub-chat).** Não existe frontend wapphub-account no roadmap aprovado.

Documentação canônica: [ADR-0001 — Fronteiras administrativas M2](docs/ADR-0001-M2-ADMIN-BOUNDARIES.md). Detalhamento histórico em `docs/SCOPE.md`; `docs/STATUS.md` registra entregas realmente implementadas.

Estado: planejamento/documentação, não equivale a implementação ou deploy.
