# Estudo de Caso - Veltis AI Platform

## Contexto

Projetos de IA exigem atenção a segurança, privacidade, avaliação, rastreabilidade e dependências externas. A arquitetura precisa evitar acoplamento direto a provedores e preservar governança sobre dados e resultados.

## Aplicação do padrão

- Usar contratos para integrações com provedores de IA.
- Registrar ADRs para decisões de modelo, avaliação e retenção.
- Separar orquestração de casos de uso de detalhes técnicos de API externa.
- Documentar riscos de privacidade, alucinação, indisponibilidade e custo.

## Resultado esperado

Uma arquitetura que permita evolução de provedores, revisão de qualidade, auditoria e operação segura sem expor detalhes sensíveis no repositório.
