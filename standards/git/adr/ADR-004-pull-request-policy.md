# ADR-004 - Exigir pull request para integração em branches protegidas

## Status

Aceito

## Data

2026-06-26

## Contexto

Integrações diretas em branches principais reduzem rastreabilidade e aumentam risco de mudanças sem revisão.

## Decisão

Exigir pull request para integração em `main` e demais branches protegidas, salvo exceções emergenciais registradas.

## Consequências

### Positivas

- Revisão técnica mais consistente.
- Histórico de discussão e aprovação.
- Melhor controle de qualidade, segurança e documentação.

### Negativas

- Pode aumentar o tempo de integração para mudanças pequenas.
- Exige disponibilidade de revisores.

## Revisão

Revisar se houver automações ou processos equivalentes que preservem o mesmo nível de controle e rastreabilidade.
