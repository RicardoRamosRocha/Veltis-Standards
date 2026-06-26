# Veltis Standards

Veltis Standards e o framework de engenharia de software da Veltis para orientar como produtos digitais devem ser documentados, planejados, implementados, testados, operados e evoluidos.

O repositorio consolida padroes reutilizaveis para equipes que trabalham com documentacao, Git, arquitetura, ASP.NET Core, banco de dados, UI, seguranca, testes, DevOps, Flutter, inteligencia artificial e checklists de qualidade. O objetivo nao e engessar a engenharia, mas criar uma base comum para decisoes melhores, revisoes mais consistentes e entregas previsiveis.

## Objetivos

- Definir uma linguagem comum para engenharia, produto e operacoes.
- Reduzir variacao desnecessaria entre projetos da Veltis.
- Acelerar onboarding tecnico com documentacao organizada e reutilizavel.
- Melhorar rastreabilidade de decisoes, requisitos, arquitetura e releases.
- Apoiar revisoes tecnicas com criterios objetivos de qualidade.
- Preservar autonomia dos times sem abrir mao de consistencia.

## Escopo

Este framework cobre padroes e guias para documentacao, Git, arquitetura, ASP.NET Core, banco de dados, interfaces digitais, seguranca, testes, DevOps, Flutter, IA e checklists.

## Estrutura do repositorio

```text
assets/          Recursos visuais e arquivos auxiliares globais.
case-studies/    Estudos de caso aplicaveis ao framework como um todo.
docs/            Documentacao central do Veltis Standards.
examples/        Exemplos globais de aplicacao dos padroes.
standards/       Modulos independentes de padroes por tema.
templates/       Modelos globais reutilizaveis.
```

Cada modulo dentro de `standards/` possui `README.md`, `MANIFEST.md`, `CHANGELOG.md`, `roadmap.md`, `backlog.md` e as pastas `docs/`, `templates/`, `examples/`, `case-studies/`, `adr/`, `releases/` e `assets/`.

## Como usar

1. Comece por `docs/01-visao-produto.md` para entender a finalidade do framework.
2. Consulte `docs/02-requisitos.md` para conhecer os requisitos funcionais e nao funcionais.
3. Use `docs/05-arquitetura.md` para compreender a organizacao dos modulos.
4. Acesse o modulo em `standards/` correspondente ao tema que deseja aplicar.
5. Utilize templates e checklists como pontos de partida, adaptando quando houver justificativa registrada.

## Principios

- Clareza antes de volume: cada documento deve ajudar uma decisao ou uma execucao.
- Padrao reutilizavel antes de preferencia individual.
- Decisoes importantes devem ser rastreaveis.
- Seguranca, privacidade, acessibilidade e operabilidade fazem parte do desenho inicial.
- Excecoes sao permitidas quando registradas, justificadas e revisadas.

## Status

Versao inicial em estruturacao. Os modulos foram criados com documentos principais para permitir evolucao incremental, revisao por tema e versionamento organizado.
