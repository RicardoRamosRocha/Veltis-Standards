# Template de Configuração GitHub do Projeto

## Repositório

- Nome: nome-do-repositorio
- Visibilidade: privada ou pública
- Responsável técnico: equipe ou pessoa

## Branch principal

- Branch padrão: `main`
- Proteção: obrigatória

## Regras de proteção

- [ ] Exigir pull request antes de merge.
- [ ] Exigir aprovação de pelo menos uma pessoa.
- [ ] Exigir checks obrigatórios quando existirem.
- [ ] Bloquear force push.
- [ ] Bloquear exclusão da branch protegida.

## Pull requests

- Template: `.github/PULL_REQUEST_TEMPLATE.md`
- Estratégia de merge: squash, merge commit ou rebase
- Revisores obrigatórios: equipe ou papel

## Issues e projetos

Descreva como issues, labels, milestones e GitHub Projects serão usados.

## Releases

Descreva como tags e GitHub Releases serão criadas.

## Segurança

- Não armazenar segredos no repositório.
- Usar GitHub Secrets para credenciais de automação.
- Revisar permissões de colaboradores periodicamente.
