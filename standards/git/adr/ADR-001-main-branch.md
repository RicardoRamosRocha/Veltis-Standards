# ADR-001 - Adotar main como branch principal

## Status

Aceito

## Data

2026-06-26

## Contexto

Projetos da Veltis precisam de uma branch principal com nome consistente, protegida e reconhecida como fonte do estado integrável ou publicável.

## Decisão

Adotar `main` como branch principal padrão para todos os repositórios Veltis.

## Consequências

### Positivas

- Consistência entre projetos.
- Melhor alinhamento com práticas atuais do GitHub.
- Base clara para tags, releases e proteção de branch.

### Negativas

- Projetos antigos podem exigir migração de branch principal.
- Automações existentes devem ser revisadas quando dependerem de outro nome.

## Revisão

Revisar apenas se a organização adotar convenção diferente de forma ampla.
