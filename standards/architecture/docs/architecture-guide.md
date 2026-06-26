# Guia de Arquitetura

## Objetivo

Este guia define como projetos da Veltis devem tomar, registrar e revisar decisões arquiteturais. A arquitetura deve apoiar evolução sustentável, clareza de responsabilidades, segurança, testabilidade e operação previsível.

## Princípios

- A arquitetura deve responder a necessidades reais de negócio e qualidade.
- Cada camada, módulo ou serviço deve possuir responsabilidade clara.
- Dependências devem apontar para abstrações estáveis sempre que isso reduzir acoplamento real.
- Decisões relevantes devem ser registradas em ADRs.
- Simplicidade deve ser preferida até que a complexidade do domínio justifique outra abordagem.
- Segurança, observabilidade, testes e operação fazem parte da arquitetura inicial.

## Documentação mínima

Todo projeto relevante deve documentar:

- contexto do sistema;
- principais módulos e responsabilidades;
- integrações externas;
- estratégia de dados;
- decisões arquiteturais significativas;
- requisitos não funcionais críticos;
- riscos, trade-offs e limites conhecidos.

## Critérios de revisão

Uma arquitetura deve ser revisada considerando:

- clareza de fronteiras;
- coerência com requisitos funcionais e não funcionais;
- acoplamento e dependências;
- facilidade de teste;
- segurança e privacidade;
- observabilidade e suporte operacional;
- custo de evolução.

## Sinais de alerta

- Regras de negócio espalhadas por UI, controllers ou infraestrutura.
- Dependências circulares entre módulos.
- Entidades de domínio dependentes de frameworks.
- Falta de fronteira entre aplicação e persistência.
- Integrações externas sem isolamento.
- Decisões importantes sem registro.
