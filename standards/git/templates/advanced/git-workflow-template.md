# Template de Workflow Git do Projeto

## Objetivo

Definir o fluxo Git oficial do projeto, incluindo branches, commits, pull requests, releases e hotfixes.

## Modelo adotado

- [ ] GitHub Flow
- [ ] Git Flow
- [ ] Fluxo híbrido justificado

## Branches

| Branch | Finalidade | Proteção | Observações |
| --- | --- | --- | --- |
| main | Código integrável e publicável | Sim | Base para releases |
| develop | Integração da próxima versão | Conforme o projeto | Usar apenas quando necessário |

## Convenção de branches temporárias

```text
feat/descricao
fix/descricao
docs/descricao
hotfix/x.y.z-descricao
```

## Commits

Formato obrigatório:

```text
tipo(escopo opcional): descrição
```

## Pull requests

Critérios mínimos:

- resumo claro;
- validação descrita;
- revisão obrigatória;
- sem segredos ou dados sensíveis;
- documentação atualizada quando aplicável.

## Releases

Defina como criar tags, release notes, changelog e responsáveis por publicação.

## Hotfixes

Explique como abrir branch, revisar, publicar patch e sincronizar linhas de desenvolvimento.
