# Exemplo Real - Arquitetura para Renova

## Objetivo

Demonstrar como aplicar o padrão arquitetural em um sistema de CRM, atendimento, EAD e gestão operacional, sem expor código sensível, dados reais ou regras privadas.

## Direção arquitetural

O projeto deve separar domínio, aplicação, infraestrutura e apresentação, preservando regras de negócio fora de controllers, telas e persistência.

## Módulos conceituais

- Pessoas e perfis.
- Atendimento e acompanhamento.
- Cursos e progresso educacional.
- Financeiro.
- Relatórios.
- Segurança e privacidade.

## Estilo recomendado

Arquitetura em camadas com princípios de Clean Architecture pode ser adequada para proteger regras de negócio e manter testabilidade.

## Critérios de revisão

- Dados pessoais tratados com cuidado.
- Regras de atendimento e progresso protegidas no domínio ou aplicação.
- Infraestrutura isolada por contratos.
- Documentação de decisões relevantes em ADRs.
