# GitHub Flow

## Objetivo

Definir um fluxo simples e contínuo para projetos que integram mudanças diretamente em `main` por meio de pull requests revisados.

## Quando usar

Use GitHub Flow em projetos com entrega contínua, documentação, bibliotecas internas, sites, APIs simples ou produtos em que `main` pode permanecer sempre integrável.

## Fluxo recomendado

1. Atualizar a branch principal.
2. Criar uma branch curta para a mudança.
3. Fazer commits semânticos.
4. Abrir pull request para `main`.
5. Executar revisão e validações.
6. Integrar com squash, merge ou rebase conforme política do projeto.
7. Criar tag ou release quando aplicável.

## Exemplo

```bash
git switch main
git pull origin main
git switch -c docs/git-guide
git add standards/git/docs/git-guide.md
git commit -m "docs: add git usage guide"
git push -u origin docs/git-guide
```

## Política para `main`

A branch `main` deve ser protegida. Recomenda-se exigir:

- pull request antes de merge;
- pelo menos uma aprovação;
- checks obrigatórios quando existirem;
- branch atualizada antes da integração;
- bloqueio de force push.

## Estratégia de merge

- Squash merge: bom para manter histórico linear e uma mudança por PR.
- Merge commit: útil quando preservar commits internos do PR for relevante.
- Rebase merge: mantém histórico linear, mas exige cuidado com conflitos.

A política deve ser definida por projeto e aplicada de forma consistente.

## Boas práticas

- Branches devem durar poucos dias sempre que possível.
- Pull requests devem ter escopo pequeno.
- Revisões devem priorizar risco, clareza e impacto.
- Mudanças grandes devem ser divididas em PRs menores.
