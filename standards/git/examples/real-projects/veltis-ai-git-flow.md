# Exemplo Real - Fluxo Git para Veltis AI Platform

## Objetivo

Demonstrar como aplicar o padrão Git em um projeto Veltis com maior criticidade, múltiplas integrações e necessidade de rastreabilidade. Este exemplo não inclui código, prompts, credenciais, dados reais ou detalhes internos da plataforma.

## Fluxo recomendado

Para o Veltis AI Platform, recomenda-se usar Git Flow ou fluxo híbrido com branch `main` protegida e branch de integração quando houver homologação formal.

Branches sugeridas:

- `main`: versão estável e publicável.
- `develop`: integração da próxima versão, quando aplicável.
- `feat/descricao`: novas capacidades.
- `fix/descricao`: correções.
- `docs/descricao`: documentação.
- `release/x.y.z`: estabilização.
- `hotfix/x.y.z-descricao`: correções urgentes.

## Exemplo de funcionalidade

```bash
git switch develop
git pull origin develop
git switch -c feat/avaliacao-respostas
git commit -m "feat(ai): add response evaluation workflow"
git push -u origin feat/avaliacao-respostas
```

## Requisitos de pull request

- Explicar impacto funcional e técnico.
- Indicar validações executadas.
- Atualizar documentação de arquitetura, segurança ou avaliação quando aplicável.
- Não incluir dados reais, prompts sensíveis, tokens ou chaves.

## Releases

Releases devem ter tag, changelog, release notes e critérios claros de rollback quando houver impacto operacional.
