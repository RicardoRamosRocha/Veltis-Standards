# Template de Gestão de Release

## Identificação

- Versão: vX.Y.Z
- Responsável: nome ou equipe
- Data prevista: AAAA-MM-DD
- Branch base: main

## Escopo

Liste funcionalidades, correções, documentação e mudanças operacionais incluídas.

## Preparação

- [ ] Pull requests relevantes integrados.
- [ ] Changelog atualizado.
- [ ] Release notes preparadas.
- [ ] Testes executados.
- [ ] Migrações documentadas.
- [ ] Riscos conhecidos registrados.

## Comandos

```bash
git switch main
git pull origin main
git log --oneline vX.Y.Z-anterior..HEAD
git tag -a vX.Y.Z -m "Release vX.Y.Z"
git push origin vX.Y.Z
```

## Publicação no GitHub

- Criar release a partir da tag.
- Colar release notes.
- Marcar como pré-release quando aplicável.

## Pós-release

- [ ] Monitorar indicadores.
- [ ] Comunicar partes interessadas.
- [ ] Registrar incidentes ou ajustes necessários.
