# ADR-003 - Recomendar monólito modular para produtos com múltiplos domínios

## Status

Aceito

## Data

2026-06-26

## Contexto

Alguns produtos precisam de módulos claros, mas não justificam a complexidade operacional de microsserviços.

## Decisão

Recomendar monólito modular para projetos com múltiplas capacidades de negócio, necessidade de implantação simples e fronteiras internas bem definidas.

## Consequências

### Positivas

- Simplicidade operacional.
- Melhor organização por domínio.
- Possibilidade futura de extração de módulos.

### Negativas

- Exige disciplina para evitar acoplamento interno.
- Pode demandar governança sobre ownership de dados.

## Critérios de revisão

Revisar quando módulos tiverem necessidades independentes de escala, deploy ou ciclo de vida.
