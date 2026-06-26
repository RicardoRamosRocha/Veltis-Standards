# Decisões Arquiteturais

## Objetivo

Definir quando e como registrar decisões arquiteturais em ADRs, preservando contexto, alternativas e consequências.

## Quando criar ADR

Crie ADR quando a decisão:

- altera estrutura do sistema;
- define tecnologia central;
- cria dependência relevante;
- afeta segurança, dados, operação ou escalabilidade;
- estabelece padrão que será reutilizado;
- possui trade-offs importantes.

## Estrutura recomendada

- Título.
- Status.
- Data.
- Contexto.
- Decisão.
- Alternativas consideradas.
- Consequências positivas e negativas.
- Critérios de revisão.

## Status possíveis

- Proposto.
- Aceito.
- Substituído.
- Depreciado.

## Boas práticas

- Registre a decisão perto do momento em que ela é tomada.
- Explique por que alternativas foram rejeitadas.
- Não use ADR para justificar decisões triviais.
- Atualize ou substitua ADRs quando o contexto mudar.

## Relação com documentação

ADRs devem ser referenciados por documentos de arquitetura, roadmap técnico e release notes quando impactarem evolução do projeto.
