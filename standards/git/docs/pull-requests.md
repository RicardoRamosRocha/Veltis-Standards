# Pull Requests

## Objetivo

Padronizar pull requests como unidade de revisão, discussão e integração de mudanças em projetos da Veltis.

## Quando abrir

Abra um pull request quando a mudança estiver coesa, revisável e pronta para receber feedback. Pull requests não precisam estar perfeitos para discussão, mas devem ser marcados como rascunho quando ainda não estiverem prontos para aprovação.

## Tamanho recomendado

Prefira PRs pequenos. Um PR deve permitir revisão em tempo razoável e ter objetivo claro. Se a mudança exigir muitas alterações, divida por etapas: preparação, implementação, testes, documentação e limpeza.

## Estrutura mínima

Um pull request deve conter:

- resumo objetivo;
- motivação da mudança;
- arquivos, módulos ou fluxos afetados;
- evidências de validação;
- riscos conhecidos;
- pendências ou decisões necessárias.

## Checklist antes de abrir

```bash
git status
git diff origin/main...HEAD
git log --oneline origin/main..HEAD
```

Confirme:

- a branch está atualizada;
- não há arquivos sensíveis;
- commits têm mensagens claras;
- documentação foi atualizada quando necessário;
- testes ou validações aplicáveis foram executados.

## Revisão

A revisão deve priorizar:

- correção funcional;
- riscos de segurança;
- impacto em arquitetura;
- clareza e manutenção;
- aderência aos padrões Veltis;
- cobertura de testes e documentação.

## Aprovação

A aprovação indica que o revisor considera a mudança aceitável para integração. Ela não transfere a responsabilidade integral da mudança para o revisor; autoria e revisão são responsabilidades complementares.

## Integração

A estratégia de merge deve seguir a política do projeto. Para projetos que preferem histórico limpo, squash merge é recomendado. Para projetos que precisam preservar histórico granular, merge commit pode ser aceito.
