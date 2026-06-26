# Exemplo - Hotfix

## Cenário

Uma validação crítica falhou em produção e precisa de correção patch.

## Criar branch

```bash
git switch main
git pull origin main
git switch -c hotfix/1.4.1-corrige-validacao-login
```

## Commit

```bash
git add src/auth/validation.cs
git commit -m "fix: correct login validation"
git push -u origin hotfix/1.4.1-corrige-validacao-login
```

## Pull request

Abrir PR para `main`, solicitar revisão prioritária e registrar validação executada.

## Tag após merge

```bash
git switch main
git pull origin main
git tag -a v1.4.1 -m "Release v1.4.1"
git push origin v1.4.1
```

## Sincronização

Se existir `develop`, aplicar a correção também nessa linha de desenvolvimento.
