# Exemplo - Fluxo de Branch

## Cenário

Uma pessoa precisa atualizar a documentação de release de um projeto.

## Comandos

```bash
git switch main
git pull origin main
git switch -c docs/release-notes-v1
git add docs/release-notes.md
git commit -m "docs: update release notes for v1"
git push -u origin docs/release-notes-v1
```

## Pull request

O pull request deve ser aberto de `docs/release-notes-v1` para `main`, com resumo da mudança e validação manual.

## Encerramento

Após o merge:

```bash
git switch main
git pull origin main
git branch -d docs/release-notes-v1
git push origin --delete docs/release-notes-v1
```
