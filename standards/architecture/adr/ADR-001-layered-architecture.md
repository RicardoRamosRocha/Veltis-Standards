# ADR-001 - Adotar arquitetura em camadas como base conceitual

## Status

Aceito

## Data

2026-06-26

## Contexto

Projetos da Veltis precisam separar responsabilidades para reduzir acoplamento e facilitar manutenção. A ausência de camadas claras favorece regras de negócio em UI, controllers ou infraestrutura.

## Decisão

Adotar arquitetura em camadas como base conceitual mínima para projetos que possuam domínio, aplicação, apresentação e infraestrutura.

## Consequências

### Positivas

- Responsabilidades mais claras.
- Melhor testabilidade.
- Menor mistura entre negócio e tecnologia.

### Negativas

- Projetos pequenos podem perceber estrutura inicial maior.
- Exige disciplina para evitar camadas artificiais.

## Critérios de revisão

Revisar quando um projeto adotar outro estilo arquitetural com justificativa registrada.
