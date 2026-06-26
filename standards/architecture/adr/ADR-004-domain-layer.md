# ADR-004 - Proteger a camada de domínio

## Status

Aceito

## Data

2026-06-26

## Contexto

Regras de negócio espalhadas por infraestrutura, UI ou controllers reduzem clareza e dificultam testes.

## Decisão

A camada de domínio deve concentrar regras, entidades, objetos de valor, políticas e invariantes centrais, sem depender de frameworks ou detalhes externos.

## Consequências

### Positivas

- Regras de negócio mais explícitas.
- Testes mais diretos.
- Menor acoplamento com tecnologia.

### Negativas

- Exige modelagem mais cuidadosa.
- Pode demandar adaptação em projetos já acoplados.

## Critérios de revisão

Revisar quando regras de negócio começarem a aparecer em camadas externas.
