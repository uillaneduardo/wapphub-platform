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

## Coordenação da consolidação WappHub (2026-10-11)

Execução e auditoria do Provider WhatsApp/Core/Chat são conduzidas **pelo Codex no homelab**, conforme `wapphub-core/docs/WHATSAPP_WEB_CONSOLIDATION_EXECUTION.md` e acompanhadas em `wapphub-core/docs/WHATSAPP_WEB_CONSOLIDATION_PROGRESS.md`. Consultar os documentos antes de trabalho cruzado; não criar plano concorrente.

**Platform está fora do escopo funcional da consolidação atual** salvo dependência concreta aprovada. Nenhuma alteração comercial, de preços, entitlements ou billing por conveniência. Fase A0–A2 é somente auditoria e proposta; mudanças funcionais apenas após aprovação única do usuário, com testes/PR e autorização de deploy. Usuário homologa interface no navegador; progresso no Core deve conter evidências e estado real da produção, não suposições.
