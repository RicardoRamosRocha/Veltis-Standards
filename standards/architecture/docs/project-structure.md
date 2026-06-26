# Estrutura de Projeto

## Objetivo

Definir critérios para organizar projetos de forma compreensível, consistente e preparada para crescimento.

## Estrutura por responsabilidade

Projetos com arquitetura em camadas podem separar responsabilidades por camada:

```text
src/
  Product.Domain/
  Product.Application/
  Product.Infrastructure/
  Product.Api/
```

## Estrutura por módulo

Projetos com monólito modular podem organizar por capacidades:

```text
src/
  Modules/
    Billing/
    Identity/
    Catalog/
  Shared/
```

## Critérios de escolha

Use estrutura por camada quando o projeto é menor ou quando a separação técnica é suficiente. Use estrutura por módulo quando existem domínios claros, ownership diferente ou crescimento funcional relevante.

## Convenções

- Pastas devem indicar responsabilidade real.
- Evite pastas genéricas como `Helpers` para tudo.
- Evite duplicar conceitos em locais diferentes.
- Testes devem acompanhar a organização principal.
- Documentação arquitetural deve explicar a escolha.

## Revisão

A estrutura está adequada quando uma pessoa nova consegue localizar o local correto para uma mudança sem depender de conhecimento informal.
