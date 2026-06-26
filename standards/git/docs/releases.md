# Releases

## Objetivo

Padronizar como projetos da Veltis planejam, registram e publicam releases usando Git e GitHub.

## Definição

Uma release é um marco versionado que comunica um conjunto de mudanças integradas, validadas e prontas para uso ou distribuição.

## Versionamento

Use versionamento semântico quando aplicável:

```text
MAJOR.MINOR.PATCH
```

- MAJOR: mudança incompatível ou estrutural.
- MINOR: nova funcionalidade compatível.
- PATCH: correção compatível.

## Preparação

Antes de publicar uma release:

```bash
git switch main
git pull origin main
git log --oneline v1.0.0..HEAD
git status
```

Verifique:

- changelog atualizado;
- release notes preparadas;
- testes e validações concluídos;
- migrações ou ações operacionais documentadas;
- riscos conhecidos registrados.

## Publicação

```bash
git tag -a v1.1.0 -m "Release v1.1.0"
git push origin v1.1.0
```

No GitHub, crie a release a partir da tag e inclua resumo, mudanças, impactos e instruções.

## Hotfix release

Correções urgentes devem gerar versão patch:

```bash
git switch main
git pull origin main
git switch -c hotfix/1.1.1-corrige-validacao
git commit -m "fix: correct validation error"
git push -u origin hotfix/1.1.1-corrige-validacao
```

Após merge em `main`, crie `v1.1.1`.

## Evidências

Release notes devem conter evidências suficientes para auditoria: versão, data, escopo, PRs relevantes, riscos, ações necessárias e responsável.
