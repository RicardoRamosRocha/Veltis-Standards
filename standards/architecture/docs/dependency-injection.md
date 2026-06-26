# Injeção de Dependência

## Objetivo

Injeção de dependência reduz acoplamento entre componentes e facilita testes, substituição de implementações e controle explícito de dependências.

## Princípio

Classes devem declarar o que precisam para cumprir sua responsabilidade. Elas não devem criar diretamente dependências complexas, integrações externas ou infraestrutura.

## Quando usar interfaces

Use interfaces quando:

- a implementação acessa recurso externo;
- existem múltiplas implementações possíveis;
- testes precisam substituir dependência;
- a dependência pertence a uma camada externa.

Evite interfaces sem propósito quando existe apenas uma implementação estável e sem benefício de abstração.

## Ciclo de vida

Defina ciclos de vida conforme responsabilidade:

- transiente para objetos leves e sem estado;
- escopo por requisição para serviços que compartilham contexto;
- singleton apenas para objetos thread-safe e sem estado mutável perigoso.

## Cuidados

- Evite service locator.
- Evite construtores com dependências demais.
- Evite injetar infraestrutura diretamente no domínio.
- Evite esconder dependências em métodos estáticos globais.

## Revisão

Uma classe com muitas dependências pode indicar responsabilidade excessiva ou falta de divisão de casos de uso.
