# Suporte e Saúde de Integrações

## Objetivo

O WappHub Admin deve permitir diagnóstico operacional sem expor segredos do cliente.

## Visão por Organization

Exibir:
- canais configurados;
- status geral;
- última validação;
- último webhook;
- último envio;
- erros recentes;
- capability summary.

## Visão por Channel

Exemplo:
- credencial: válida/inválida/desconhecida;
- conta Meta: acesso OK/falha;
- número: resolvido/falha;
- webhook: estado;
- worker/fila: estado;
- texto: capability/health;
- imagem: capability/health;
- áudio: capability/health.

## Segurança

Nunca mostrar token completo ou permitir ao suporte copiar segredo em claro por padrão.

Diagnóstico e observabilidade devem substituir a exposição de credenciais.

## Ações de suporte

Permitidas conforme permission:
- executar diagnóstico;
- consultar histórico de diagnostic runs;
- consultar erros sanitizados;
- verificar capabilities;
- orientar contratante.

Alterações de configuração/credenciais devem ser auditadas e, idealmente, realizadas pelo Owner da Organization quando possível.
