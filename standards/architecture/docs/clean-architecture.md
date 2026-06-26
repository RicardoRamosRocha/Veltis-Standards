# Clean Architecture

## Objetivo

Clean Architecture organiza o sistema ao redor do domínio e dos casos de uso, mantendo frameworks, bancos e interfaces como detalhes externos.

## Regra central

Dependências devem apontar para dentro. O domínio não deve depender de banco de dados, UI, APIs externas ou frameworks.

## Elementos

### Domain

Entidades, objetos de valor, regras de negócio e contratos conceituais.

### Application

Casos de uso, comandos, consultas, validações de fluxo, interfaces de portas e orquestração.

### Infrastructure

Implementações de repositórios, provedores externos, mensageria, arquivos, cache e persistência.

### Presentation

APIs, UI, endpoints, controllers ou adaptadores de entrada.

## Quando usar

Use quando o projeto possui domínio com regras importantes, expectativa de evolução, necessidade de testes e dependências externas relevantes.

## Trade-offs

Clean Architecture aumenta disciplina estrutural e testabilidade, mas pode adicionar complexidade inicial. Em sistemas muito simples, uma arquitetura em camadas mais direta pode ser suficiente.

## Aplicação prática

- Defina casos de uso antes de detalhes de infraestrutura.
- Use interfaces quando houver dependência externa relevante.
- Mantenha regras de domínio fora de controllers e ORMs.
- Teste casos de uso sem depender de banco real quando possível.
