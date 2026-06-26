# Guia Git

## Objetivo

Este guia define o uso esperado de Git em projetos da Veltis. O objetivo é manter histórico legível, colaboração previsível, rastreabilidade entre mudança e decisão, e segurança no processo de entrega.

## Princípios

- A branch `main` deve representar o estado integrável e protegido do projeto.
- Mudanças devem ser pequenas, revisáveis e associadas a um objetivo claro.
- Commits devem explicar intenção, não apenas listar arquivos alterados.
- Pull requests devem ser o mecanismo padrão de revisão antes de integrar mudanças.
- Releases devem ser rastreáveis por tags, changelog ou release notes.
- Segredos, tokens, senhas e dados sensíveis nunca devem ser versionados.

## Configuração inicial recomendada

```bash
git config --global user.name "Nome Sobrenome"
git config --global user.email "email@empresa.com"
git config --global init.defaultBranch main
git config --global pull.rebase false
git config --global core.autocrlf true
```

Em Windows, `core.autocrlf true` reduz fricção com finais de linha. Em Linux ou macOS, avalie `input` conforme o projeto.

## Ciclo básico de trabalho

```bash
git status
git switch main
git pull origin main
git switch -c feat/nome-curto-da-mudanca
git add caminho/do/arquivo.md
git commit -m "docs: describe documentation workflow"
git push -u origin feat/nome-curto-da-mudanca
```

Depois do push, abra um pull request no GitHub, solicite revisão e integre somente após validações necessárias.

## Verificação antes de commitar

```bash
git status
git diff
git diff --cached
git log --oneline -5
```

Use `git diff` para revisar mudanças ainda não adicionadas ao índice. Use `git diff --cached` para revisar exatamente o que entrará no commit.

## Arquivos sensíveis

Antes de commitar, confirme que não há:

- `.env` com valores reais;
- tokens, senhas, chaves privadas ou certificados;
- dumps de banco ou dados pessoais;
- logs com informações sensíveis;
- arquivos gerados que não devem ser versionados.

## Recuperação segura

Prefira comandos não destrutivos para desfazer alterações:

```bash
git restore caminho/do/arquivo.md
git restore --staged caminho/do/arquivo.md
git revert <sha-do-commit>
```

Evite `git reset --hard` sem alinhamento explícito, pois ele descarta alterações locais.
