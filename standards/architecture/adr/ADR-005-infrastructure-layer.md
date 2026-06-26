# ADR-005 - Isolar detalhes na camada de infraestrutura

## Status

Aceito

## Data

2026-06-26

## Contexto

Bancos de dados, provedores externos, mensageria, arquivos e serviços técnicos mudam com mais frequência que regras de negócio.

## Decisão

A camada de infraestrutura deve concentrar implementações técnicas e depender de contratos definidos por camadas internas quando necessário.

## Consequências

### Positivas

- Detalhes externos ficam isolados.
- Substituição de provedores se torna mais segura.
- Testes podem substituir implementações externas.

### Negativas

- Exige definição clara de contratos.
- Pode criar complexidade se usada sem necessidade real.

## Critérios de revisão

Revisar quando detalhes de infraestrutura vazarem para domínio ou aplicação.
