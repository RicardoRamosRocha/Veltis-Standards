# Repository Pattern

## Objetivo

Repository Pattern encapsula acesso a dados e oferece uma abstração orientada ao domínio ou ao caso de uso, reduzindo acoplamento com persistência.

## Quando usar

Use quando o domínio precisa ser protegido de detalhes de banco, ORM ou origem de dados, ou quando consultas e persistência precisam ser testáveis.

## Responsabilidade

Um repositório deve:

- recuperar e persistir agregados ou modelos necessários;
- esconder detalhes de consulta e armazenamento;
- expor operações com significado para o domínio ou aplicação.

## O que evitar

- Repositórios genéricos que apenas replicam operações do ORM sem valor.
- Regras de negócio dentro do repositório.
- Expor detalhes de infraestrutura para a camada de domínio.
- Métodos excessivamente genéricos que dificultam revisão.

## Consultas

Consultas complexas de leitura podem usar objetos ou serviços específicos de consulta, especialmente quando não representam agregados de domínio.

## Exemplo conceitual

```text
Application -> Contract -> Infrastructure implementation -> Database
```

A aplicação depende do contrato, e a infraestrutura fornece a implementação.
