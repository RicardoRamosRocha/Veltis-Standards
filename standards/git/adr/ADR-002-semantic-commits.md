# ADR-002 - Adotar commits semânticos

## Status

Aceito

## Data

2026-06-26

## Contexto

Mensagens de commit genéricas dificultam revisão, auditoria, investigação de regressões e geração de changelog.

## Decisão

Adotar commits semânticos no formato `tipo(escopo opcional): descrição`.

## Consequências

### Positivas

- Histórico mais legível.
- Melhor rastreabilidade por tipo de mudança.
- Facilita automações futuras de changelog e release.

### Negativas

- Exige disciplina de escrita.
- Pode exigir ajustes em commits antes do merge.

## Revisão

Revisar se a Veltis adotar ferramenta formal de versionamento que exija convenção diferente.
