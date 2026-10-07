# Escopo do WappHub Platform

A aplicação possui dois contextos.

## 1. WappHub Admin

Uso interno da WappHub.

MVP:
- listar/cadastrar/editar Organizations;
- gerenciar Products;
- gerenciar Plans;
- aceitar preço R$ 0,00;
- gerenciar Features;
- vincular Features a Plans;
- configurar quantidades incluídas;
- criar/alterar/suspender Subscriptions;
- visualizar/adicionar assentos/add-ons;
- criar overrides/cortesias auditáveis;
- visualizar saúde das integrações por Organization/Channel;
- executar/consultar diagnósticos conforme permission;
- visualizar capabilities sem expor segredos;
- visualizar auditoria administrativa.

Detalhes de suporte: `docs/INTEGRATION_SUPPORT.md`.

## 2. Minha Conta

Uso do Owner autorizado de uma Organization.

MVP:
- visualizar organização atual;
- visualizar assinatura;
- plano atual;
- recursos efetivos;
- assentos contratados;
- assentos utilizados;
- assentos disponíveis;
- faturamento básico;
- conta pessoal.

Configuração operacional do canal WhatsApp permanece no Chat/área operacional apropriada; o Platform exibe informações comerciais e de suporte conforme papel.

## Separação

O Platform não é a interface de atendimento. Conversas e operação diária pertencem ao `wapphub-chat`.

O WappHub Admin não usa exceções hardcoded para a própria WappHub. A WappHub deve existir como Organization cliente com Subscription normal, inclusive plano de R$ 0,00.

## Segurança

Admin pode diagnosticar integração sem obter token Meta em claro.

Mudanças administrativas de subscription, feature, entitlement e integração precisam ser auditáveis.
