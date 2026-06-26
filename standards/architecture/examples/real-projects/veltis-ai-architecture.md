# Exemplo Real - Arquitetura para Veltis AI Platform

## Objetivo

Demonstrar como aplicar o padrão arquitetural em um projeto de inteligência artificial da Veltis sem expor código, prompts, dados reais, credenciais ou detalhes internos.

## Direção arquitetural

O projeto deve priorizar separação clara entre domínio de produto, orquestração de casos de uso, integrações com provedores de IA, avaliação, segurança e observabilidade.

## Módulos conceituais

- Identidade e acesso.
- Orquestração de interações de IA.
- Avaliação e qualidade de respostas.
- Governança e auditoria.
- Integrações externas.
- Observabilidade operacional.

## Decisões recomendadas

- Registrar ADRs para escolha de provedores, estratégia de avaliação e retenção de dados.
- Isolar provedores externos por contratos.
- Tratar prompts, dados e logs como ativos sensíveis.
- Separar regras de negócio de detalhes de modelo ou API externa.

## Critérios de revisão

A arquitetura deve demonstrar rastreabilidade, proteção de dados, capacidade de avaliação e possibilidade de substituição controlada de dependências externas.
