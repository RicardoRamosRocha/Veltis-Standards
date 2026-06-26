# Commits

## Objetivo

Definir mensagens de commit claras e semânticas, preservando histórico útil para revisão, auditoria, changelog e investigação de problemas.

## Formato recomendado

```text
tipo: descrição objetiva no imperativo ou infinitivo curto
```

Exemplos:

```bash
git commit -m "docs: add git branch conventions"
git commit -m "fix: correct release tag validation"
git commit -m "feat: add user invitation workflow"
git commit -m "test: cover authentication failure scenario"
```

## Tipos comuns

- `feat`: nova funcionalidade.
- `fix`: correção de defeito.
- `docs`: documentação.
- `style`: formatação sem mudança de comportamento.
- `refactor`: reestruturação interna sem mudança funcional.
- `test`: testes.
- `chore`: manutenção, build, dependências ou tarefas auxiliares.
- `ci`: pipeline e integração contínua.
- `perf`: desempenho.
- `security`: melhoria ou correção de segurança.

## Escopo opcional

Quando útil, inclua escopo:

```bash
git commit -m "docs(git): add pull request policy"
git commit -m "fix(api): validate required customer id"
```

## Corpo do commit

Use corpo quando a mudança exigir contexto:

```bash
git commit -m "docs: define release branch policy" -m "Explica quando usar release branches e como sincronizar main e develop após publicação."
```

## Commits pequenos

Um commit deve representar uma unidade lógica de mudança. Evite misturar documentação, refatoração, funcionalidade e correção sem relação.

## Antes do commit

```bash
git status
git diff
git add caminho/do/arquivo.md
git diff --cached
git commit -m "docs: update git commit guide"
```

## O que evitar

- `git commit -m "ajustes"`
- `git commit -m "final"`
- `git commit -m "corrige coisas"`
- commits com segredos ou arquivos gerados indevidos.
