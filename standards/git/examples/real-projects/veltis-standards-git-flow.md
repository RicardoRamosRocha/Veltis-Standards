# Exemplo Real - Fluxo Git para Veltis Standards

## Objetivo

Demonstrar como aplicar o padrão Git no próprio repositório Veltis Standards.

## Fluxo recomendado

O Veltis Standards pode usar GitHub Flow, pois é um framework documental versionado e as mudanças devem ser integradas em `main` por pull requests revisados.

## Branches

Exemplos:

```bash
git switch main
git pull origin main
git switch -c docs/git-module-v1
git switch -c docs/security-baseline
git switch -c chore/audit-release-readiness
```

## Commits

Mensagens recomendadas:

```bash
git commit -m "docs: complete git standard module v1"
git commit -m "docs: audit repository and improve documentation consistency"
```

## Pull requests

Cada PR deve manter escopo claro. Uma sprint de módulo deve alterar apenas o módulo correspondente e documentos globais autorizados.

## Releases

A Release 1.0 global deve ser marcada com tag quando os módulos críticos atingirem maturidade suficiente e o changelog global estiver consolidado.
