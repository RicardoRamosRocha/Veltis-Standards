# Template Git para Múltiplos Ambientes

## Objetivo

Definir como branches, tags e releases se relacionam com ambientes de desenvolvimento, homologação e produção.

## Ambientes

| Ambiente | Origem | Publicação | Observações |
| --- | --- | --- | --- |
| Desenvolvimento | develop ou branch de feature | Automática ou manual | Quando aplicável |
| Homologação | release/x.y.z | Manual ou controlada | Usada para validação formal |
| Produção | main + tag | Controlada | Somente versão aprovada |

## Fluxo recomendado

1. Desenvolver em branch temporária.
2. Integrar em `develop` ou `main`, conforme fluxo adotado.
3. Criar branch `release/x.y.z` quando houver homologação formal.
4. Validar release.
5. Integrar em `main`.
6. Criar tag `vX.Y.Z`.
7. Publicar release.

## Hotfix

Correções urgentes devem nascer de `main`:

```bash
git switch main
git pull origin main
git switch -c hotfix/x.y.z-descricao
```

Após integração, sincronize a correção com a linha de desenvolvimento ativa.

## Regras

- Ambientes produtivos devem usar tags ou commits rastreáveis.
- Deploy manual deve registrar versão publicada.
- Branch de ambiente não deve acumular mudanças manuais permanentes.
