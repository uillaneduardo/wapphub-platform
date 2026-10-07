# Instruções para agentes e Codex — WappHub Platform

Leia README.md, docs/SCOPE.md, docs/ROUTES.md e docs/STATUS.md antes de alterar código.

## Regras

- Não implementar lógica de domínio comercial no frontend.
- Não liberar funcionalidades com base no nome do plano.
- Preço 0 é válido.
- WappHub Admin e Minha Conta são contextos de UI distintos.
- Conversas/atendimento pertencem ao wapphub-chat.
- Toda alteração de assinatura/recurso deve usar APIs do Core e ser auditável.
- Menus e rotas respeitam permissions.
- Não implementar billing recorrente completo antes de milestone específico.
- Atualizar docs/STATUS.md quando uma funcionalidade for realmente entregue.
