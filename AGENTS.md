# Instruções para agentes e Codex — WappHub Platform

Leia README.md, docs/SCOPE.md, docs/ROUTES.md, docs/INTEGRATION_SUPPORT.md e docs/STATUS.md antes de alterar código.

## Regras

- Não implementar lógica de domínio comercial no frontend.
- Não liberar funcionalidades pelo nome do plano.
- Preço 0 é válido.
- WappHub Admin e Minha Conta são contextos de UI distintos.
- Conversas/atendimento pertencem ao wapphub-chat.
- Toda alteração de assinatura/recurso usa APIs do Core e é auditável.
- Menus e rotas respeitam permissions.
- Não implementar billing recorrente completo antes de milestone próprio.
- Diagnóstico deve usar dados estruturados do Core.
- Nunca exibir ou recuperar token Meta completo no frontend de suporte.
- Saúde da integração não deve ser confundida com entitlement.
- Não marcar STATUS como concluído sem validação.
