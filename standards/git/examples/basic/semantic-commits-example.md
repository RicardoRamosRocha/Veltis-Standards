# Exemplo - Commits Semânticos

## Objetivo

Demonstrar mensagens de commit claras e rastreáveis.

## Bons exemplos

```bash
git commit -m "docs: add git release guide"
git commit -m "feat(auth): add password reset flow"
git commit -m "fix(api): return 404 when customer does not exist"
git commit -m "test(payments): cover failed transaction scenario"
git commit -m "chore: update dependency lock file"
```

## Exemplo com corpo

```bash
git commit -m "docs: define pull request policy" -m "Inclui critérios de revisão, validação e integração para projetos Veltis."
```

## Exemplos ruins

```bash
git commit -m "ajustes"
git commit -m "final"
git commit -m "coisas"
```

Essas mensagens não explicam intenção, escopo ou impacto.
