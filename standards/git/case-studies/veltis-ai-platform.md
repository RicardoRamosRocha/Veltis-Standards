# Estudo de Caso - Veltis AI Platform

## Contexto

O Veltis AI Platform é um exemplo de projeto com maior criticidade técnica, pois pode envolver integrações, governança de IA, segurança, privacidade, avaliação e operação contínua.

Este estudo descreve apenas a aplicação do padrão Git. Não inclui código, prompts, dados reais, credenciais ou detalhes internos da plataforma.

## Fluxo recomendado

Projetos com esse perfil devem usar Git Flow ou fluxo híbrido quando houver homologação formal antes de produção. A branch `main` deve representar a versão estável e publicável.

## Regras essenciais

- Pull requests obrigatórios para `main`.
- Revisão técnica para mudanças de arquitetura, segurança ou avaliação de IA.
- Tags para releases formais.
- Release notes com impactos e riscos conhecidos.
- Proibição de segredos, tokens, prompts sensíveis ou dados reais no repositório.

## Exemplo de hotfix

```bash
git switch main
git pull origin main
git switch -c hotfix/1.3.1-corrige-avaliacao
git commit -m "fix(ai): correct evaluation fallback behavior"
git push -u origin hotfix/1.3.1-corrige-avaliacao
```

## Benefícios

- Maior controle de mudanças críticas.
- Rastreabilidade entre PR, tag e release.
- Separação clara entre desenvolvimento, estabilização e correção urgente.
- Melhor suporte para auditoria e governança.
