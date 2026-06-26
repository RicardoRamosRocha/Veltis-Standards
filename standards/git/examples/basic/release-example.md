# Exemplo - Release

## Cenário

Publicar a versão `v1.2.0` de um projeto após integração dos PRs planejados.

## Verificação

```bash
git switch main
git pull origin main
git log --oneline v1.1.0..HEAD
git status
```

## Criar tag

```bash
git tag -a v1.2.0 -m "Release v1.2.0"
git push origin v1.2.0
```

## Release notes

Resumo:

- novas funcionalidades de cadastro;
- correções de validação;
- atualização da documentação de API.

## Pós-release

- Confirmar publicação no GitHub Releases.
- Comunicar partes interessadas.
- Monitorar erros e indicadores.
