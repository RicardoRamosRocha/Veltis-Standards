# Service Layer

## Objetivo

A camada de serviços organiza operações de aplicação ou domínio, evitando que controllers, componentes de UI ou infraestrutura concentrem regras e orquestração.

## Tipos de serviço

### Serviço de aplicação

Orquestra casos de uso, valida fluxo, chama repositórios, publica eventos e coordena transações.

### Serviço de domínio

Representa regra de negócio que não pertence naturalmente a uma entidade ou objeto de valor.

### Serviço de infraestrutura

Implementa detalhes técnicos como e-mail, armazenamento, mensageria, APIs externas ou arquivos.

## Boas práticas

- Nomeie serviços pela responsabilidade, não pela tecnologia.
- Evite serviços grandes demais.
- Separe orquestração de regra de negócio.
- Não transforme serviços em repositórios disfarçados.

## Sinais de alerta

- Serviço com métodos sem relação entre si.
- Serviço que apenas repassa chamadas sem agregar regra ou coordenação.
- Serviço de aplicação contendo detalhes de SQL, HTTP externo ou framework.

## Revisão

Um serviço é adequado quando sua responsabilidade pode ser explicada em uma frase clara e seus métodos estão conectados a essa responsabilidade.
