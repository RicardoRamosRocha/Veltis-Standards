# Exemplo - Clean Architecture

## Cenário

Produto com regras de cadastro, aprovação e auditoria.

## Organização conceitual

```text
Domain: entidades, objetos de valor e políticas.
Application: casos de uso como AprovarCadastro.
Infrastructure: repositórios, e-mail e banco.
Presentation: API e interface administrativa.
```

## Decisão

O domínio não depende de ORM, API ou framework. A aplicação depende de contratos, e a infraestrutura implementa esses contratos.

## Benefícios

- Testes de domínio sem infraestrutura.
- Troca de tecnologia externa com menor impacto.
- Regras de negócio mais visíveis.
