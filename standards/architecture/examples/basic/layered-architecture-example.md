# Exemplo - Arquitetura em Camadas

## Contexto

Sistema administrativo com API, regras de negócio e persistência relacional.

## Estrutura conceitual

```text
Api -> Application -> Domain
Api -> Infrastructure
Application -> Infrastructure contracts
Infrastructure -> Database and external services
```

## Responsabilidades

- Api: recebe requisições e retorna respostas.
- Application: executa casos de uso.
- Domain: protege regras e invariantes.
- Infrastructure: implementa persistência e integrações.

## Critério de qualidade

Uma regra de negócio deve estar no domínio ou em serviço de domínio, não em controller ou componente visual.
