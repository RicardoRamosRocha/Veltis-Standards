# Branches

## Objetivo

Padronizar nomes, finalidade e ciclo de vida de branches em projetos da Veltis.

## Convenção de nomes

Use nomes curtos, em minúsculas, sem acentos e com hífen para separar palavras.

Formato recomendado:

```text
tipo/descricao-curta
```

Tipos recomendados:

- `feat/`: nova funcionalidade.
- `fix/`: correção de defeito.
- `docs/`: documentação.
- `chore/`: manutenção, configuração ou tarefas auxiliares.
- `refactor/`: melhoria interna sem mudança de comportamento.
- `test/`: inclusão ou ajuste de testes.
- `release/`: estabilização de versão.
- `hotfix/`: correção urgente baseada em produção.

## Exemplos

```bash
git switch -c feat/autenticacao-sso
git switch -c fix/validacao-cpf
git switch -c docs/padrao-git
git switch -c chore/atualiza-dependencias
git switch -c hotfix/1.0.1-corrige-sessao-expirada
```

## Branches protegidas

`main` deve ser protegida. Quando existir `develop`, ela também deve ter regras de proteção compatíveis com o risco do projeto.

## Ciclo de vida

Branches temporárias devem ser removidas após merge:

```bash
git branch -d docs/padrao-git
git push origin --delete docs/padrao-git
```

## O que evitar

- nomes como `ajustes`, `teste`, `minha-branch` ou `final`;
- branches longas sem sincronização;
- uso de nome de pessoa como finalidade da branch;
- branch com escopo maior que um PR revisável.
