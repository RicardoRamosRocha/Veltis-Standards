# Estudo de Caso - Veltis Standards

## Contexto

O Veltis Standards é um framework documental e modular. Seu fluxo Git precisa favorecer rastreabilidade, revisão de conteúdo e evolução incremental dos módulos.

## Decisão de fluxo

O fluxo recomendado é GitHub Flow com `main` protegida. Cada sprint documental deve ser desenvolvida em branch própria e integrada por pull request.

## Aplicação prática

Exemplos de branches:

```bash
git switch -c docs/documentation-module-v1
git switch -c docs/git-module-v1
git switch -c docs/release-audit
```

Exemplos de commits:

```bash
git commit -m "docs: complete documentation standard module v1"
git commit -m "docs: complete git standard module v1"
```

## Critérios de revisão

- Escopo restrito ao módulo ou documento autorizado.
- Conteúdo em português e Markdown.
- Sem dados sensíveis.
- Estrutura compatível com o padrão do repositório.
- Changelog e roadmap atualizados quando necessário.

## Benefícios

- Histórico claro por sprint.
- Revisão objetiva.
- Preparação gradual para Release 1.0.
- Rastreabilidade de decisões e auditorias.
