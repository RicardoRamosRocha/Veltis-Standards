# Git Flow

## Objetivo

Definir como usar um fluxo estruturado de branches quando o projeto precisar separar desenvolvimento, homologação, releases e correções urgentes.

## Quando usar

Use Git Flow quando o projeto possui ciclos de release planejados, múltiplos ambientes, homologação formal ou manutenção simultânea de versões.

Para projetos simples, bibliotecas internas pequenas ou documentação, o GitHub Flow pode ser suficiente.

## Branches principais

- `main`: versão estável, protegida e publicável.
- `develop`: integração contínua de funcionalidades antes da próxima release, quando o projeto exigir essa separação.
- `release/x.y.z`: estabilização de uma versão.
- `hotfix/x.y.z-descricao`: correção urgente baseada em `main`.
- `feat/descricao`: desenvolvimento de funcionalidade.
- `fix/descricao`: correção não emergencial.
- `docs/descricao`: alteração documental.
- `chore/descricao`: manutenção sem impacto funcional direto.

## Fluxo de funcionalidade

```bash
git switch develop
git pull origin develop
git switch -c feat/cadastro-de-usuarios
# editar arquivos
git add .
git commit -m "feat: add user registration flow"
git push -u origin feat/cadastro-de-usuarios
```

Abra pull request para `develop`. Após revisão e validações, integre a mudança.

## Fluxo de release

```bash
git switch develop
git pull origin develop
git switch -c release/1.2.0
# ajustes finais, changelog e versionamento
git commit -m "chore: prepare release 1.2.0"
git push -u origin release/1.2.0
```

Após homologação, integre em `main`, crie tag e sincronize `develop`.

## Fluxo de hotfix

```bash
git switch main
git pull origin main
git switch -c hotfix/1.2.1-corrige-login
git add .
git commit -m "fix: correct login validation"
git push -u origin hotfix/1.2.1-corrige-login
```

O pull request deve ir para `main`. Depois da integração, a correção deve ser refletida na linha de desenvolvimento ativa.

## Cuidados

- Não mantenha branches longas sem sincronização.
- Não use `develop` se ele não tiver função real no projeto.
- Não publique release sem changelog ou release notes quando houver impacto para usuários.
- Não force push em branches compartilhadas sem alinhamento explícito.
