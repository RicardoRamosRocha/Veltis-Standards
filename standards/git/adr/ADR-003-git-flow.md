# ADR-003 - Usar GitHub Flow por padrão e Git Flow quando necessário

## Status

Aceito

## Data

2026-06-26

## Contexto

Projetos da Veltis variam em complexidade. Alguns precisam de homologação formal e múltiplas linhas de desenvolvimento; outros exigem fluxo simples com integração contínua em `main`.

## Decisão

Adotar GitHub Flow como fluxo padrão para projetos simples, documentais ou de entrega contínua. Usar Git Flow ou fluxo híbrido quando houver releases planejadas, homologação formal, múltiplos ambientes ou manutenção simultânea de versões.

## Consequências

### Positivas

- Evita complexidade desnecessária em projetos simples.
- Permite governança adequada em projetos críticos.
- Dá autonomia com critérios claros de escolha.

### Negativas

- Exige que cada projeto declare o fluxo adotado.
- Pode haver variação controlada entre equipes.

## Revisão

Revisar após adoção em projetos reais e coleta de evidências de fricção ou risco.
