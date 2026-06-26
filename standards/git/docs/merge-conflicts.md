# Conflitos de Merge

## Objetivo

Orientar resolução segura de conflitos de merge, reduzindo risco de perda de trabalho e regressões.

## Prevenção

- Mantenha branches curtas.
- Sincronize frequentemente com `main` ou `develop`.
- Evite alterar arquivos grandes e compartilhados sem alinhamento.
- Divida mudanças extensas em PRs menores.

## Identificar conflitos

```bash
git status
```

Arquivos em conflito aparecem como `both modified`, `added by us`, `deleted by them` ou situações semelhantes.

## Atualizar branch antes de resolver

```bash
git fetch origin
git merge origin/main
```

Ou, se o projeto usa rebase:

```bash
git fetch origin
git rebase origin/main
```

Use a estratégia definida pelo projeto.

## Resolver conflito

Abra o arquivo conflitante e procure marcadores:

```text
<<<<<<< HEAD
conteúdo atual
=======
conteúdo recebido
>>>>>>> origin/main
```

Edite o arquivo para manter o resultado correto, remova os marcadores e valide o conteúdo final.

## Finalizar merge

```bash
git add caminho/do/arquivo.md
git commit
```

## Finalizar rebase

```bash
git add caminho/do/arquivo.md
git rebase --continue
```

Para abortar com segurança:

```bash
git merge --abort
git rebase --abort
```

## Validação

Após resolver conflitos, execute testes, revisão documental ou validações aplicáveis. Conflitos resolvidos manualmente devem receber atenção extra em revisão.
