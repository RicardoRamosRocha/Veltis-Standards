# Domain-Driven Design

## Objetivo

Domain-Driven Design orienta a modelagem do software a partir do domínio de negócio, linguagem comum e limites claros de contexto.

## Linguagem ubíqua

Equipes técnicas e de negócio devem usar os mesmos termos para conceitos centrais. Esses termos devem aparecer em documentos, código, APIs e conversas de refinamento.

## Bounded Context

Um contexto delimitado define onde um modelo é válido. O mesmo termo pode ter significados diferentes em contextos distintos, e isso deve ser documentado.

## Entidades

Representam conceitos com identidade contínua ao longo do tempo.

## Objetos de valor

Representam valores sem identidade própria, definidos por seus atributos.

## Agregados

Agrupam entidades e objetos de valor que precisam manter consistência transacional.

## Serviços de domínio

Representam regras de negócio que não pertencem naturalmente a uma entidade ou objeto de valor.

## Quando aplicar

Use DDD quando o domínio é complexo, possui linguagem rica, regras relevantes e exige colaboração próxima com especialistas de negócio.

## Cuidados

- Não aplicar DDD apenas por estética arquitetural.
- Não criar agregados grandes demais.
- Não deixar o modelo de banco definir o modelo de domínio.
- Registrar decisões sobre limites de contexto.
