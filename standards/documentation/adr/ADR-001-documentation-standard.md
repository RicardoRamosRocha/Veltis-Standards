# ADR-001 - Adotar padrão único de documentação para projetos Veltis

## Status

Aceito

## Data

2026-06-26

## Contexto

Projetos da Veltis precisam registrar visão de produto, requisitos, arquitetura, decisões, APIs, releases e processos de operação de forma consistente. Sem um padrão único, cada equipe tende a criar estruturas próprias, dificultando onboarding, revisão técnica, rastreabilidade e manutenção.

A ausência de padronização também aumenta o risco de documentação incompleta, duplicada ou desatualizada, especialmente em projetos com múltiplas áreas envolvidas.

## Decisão

Adotar o módulo `standards/documentation` como padrão oficial de documentação para todos os projetos da Veltis. O módulo define guias, princípios, ciclo de vida, convenções, templates, exemplos, processo de revisão e critérios de versionamento documental.

## Alternativas consideradas

### Manter documentação livre por projeto

Permite autonomia máxima, mas aumenta variação, dificulta revisão e reduz previsibilidade entre equipes.

### Usar apenas uma ferramenta externa de documentação

Melhora publicação e colaboração visual, mas não garante estrutura, versionamento junto ao repositório nem revisão no fluxo de mudanças.

### Definir somente templates mínimos

Ajuda a iniciar documentos, mas não resolve filosofia, ciclo de vida, revisão, nomenclatura e governança.

## Consequências

### Positivas

- Estrutura documental previsível entre projetos.
- Melhor onboarding técnico e funcional.
- Revisões documentais mais objetivas.
- Rastreabilidade entre decisões, requisitos, mudanças e releases.
- Base reutilizável para projetos simples e complexos.

### Negativas

- Projetos existentes precisarão adaptar documentos gradualmente.
- Pessoas mantenedoras precisarão revisar o padrão periodicamente.
- Exceções deverão ser registradas para evitar uso mecânico do padrão.

## Diretrizes de adoção

Novos projetos devem iniciar com os templates básicos ou avançados do módulo. Projetos existentes devem migrar de forma incremental, priorizando README, visão de produto, requisitos, arquitetura, changelog e ADRs relevantes.

## Revisão

Esta decisão deve ser revisada quando o padrão deixar de atender aos principais tipos de projeto da Veltis ou quando a organização adotar uma plataforma documental que altere o fluxo de manutenção.
