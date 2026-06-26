# Arquitetura do Framework

## Visao geral

O Veltis Standards e organizado como um framework documental modular. A arquitetura do repositorio separa documentos globais, modulos de padrao, templates, exemplos e estudos de caso para permitir evolucao independente e consulta rapida.

A unidade principal de organizacao e o modulo em `standards/`. Cada modulo representa um dominio de padronizacao e possui arquivos de governanca, evolucao e conteudo proprio.

## Camadas documentais

### Documentacao central

A pasta `docs/` descreve o framework como produto interno: visao, requisitos, backlog, roadmap, arquitetura e organizacao. Ela responde por contexto, governanca geral e criterios que atravessam todos os modulos.

### Modulos de padrao

A pasta `standards/` contem os dominios reutilizaveis. Cada modulo deve ser tratavel como uma unidade evolutiva, com backlog, roadmap, changelog e manifesto proprio.

### Artefatos reutilizaveis

As pastas `templates/`, `examples/`, `case-studies/` e `assets/` existem em nivel global e dentro dos modulos. O nivel global deve conter materiais aplicaveis a multiplos modulos; o nivel do modulo deve conter materiais especificos do dominio.

## Contrato de modulo

Todo modulo deve preservar a estrutura definida em `standards/<modulo>/`, com arquivos principais e pastas para documentos, templates, exemplos, estudos de caso, ADRs, releases e assets.

## Relacionamento entre modulos

Modulos podem se referenciar, mas nao devem duplicar responsabilidades. Quando um tema depender de outro, o documento deve apontar para o modulo responsavel e explicar o relacionamento.

Exemplos:

- `aspnet-core` depende de criterios de `security`, `testing`, `architecture` e `devops`.
- `database` depende de `security`, `architecture` e `devops`.
- `ui` e `flutter` compartilham principios de experiencia, acessibilidade e consistencia visual.
- `ai` depende de seguranca, privacidade, avaliacao e rastreabilidade.

## Governanca arquitetural

Mudancas que alteram estrutura, contrato de modulo, obrigatoriedade de artefatos ou criterios globais devem ser tratadas como mudancas arquiteturais do framework. Elas exigem justificativa, atualizacao do changelog e, quando apropriado, registro de decisao.
