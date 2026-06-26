# Arquitetura do Framework

## VISÃO geral

O Veltis Standards e organizado como um framework documental modular. A arquitetura do REPOSITÓRIO separa documentos globais, MÓDULOS de PADRÃO, templates, exemplos e estudos de caso para permitir EVOLUÇÃO independente e consulta rapida.

A unidade principal de ORGANIZAÇÃO e o MÓDULO em `standards/`. Cada MÓDULO representa um DOMÍNIO de padronizacao e possui arquivos de governanca, EVOLUÇÃO e CONTEÚDO PRÓPRIO.

## Camadas documentais

### DOCUMENTAÇÃO central

A pasta `docs/` descreve o framework como produto interno: VISÃO, requisitos, backlog, roadmap, arquitetura e ORGANIZAÇÃO. Ela responde por contexto, governanca geral e CRITÉRIOS que atravessam todos os MÓDULOS.

### MÓDULOS de PADRÃO

A pasta `standards/` contem os DOMÍNIOS reutilizaveis. Cada MÓDULO deve ser tratavel como uma unidade evolutiva, com backlog, roadmap, changelog e manifesto PRÓPRIO.

### Artefatos reutilizaveis

As pastas `templates/`, `examples/`, `case-studies/` e `assets/` existem em NÍVEL global e dentro dos MÓDULOS. O NÍVEL global deve conter materiais APLICÁVEIS a multiplos MÓDULOS; o NÍVEL do MÓDULO deve conter materiais especificos do DOMÍNIO.

## Contrato de MÓDULO

Todo MÓDULO deve preservar a estrutura definida em `standards/<modulo>/`, com arquivos principais e pastas para documentos, templates, exemplos, estudos de caso, ADRs, releases e assets.

## Relacionamento entre MÓDULOS

MÓDULOS podem se referenciar, mas NÃO devem duplicar responsabilidades. Quando um tema depender de outro, o documento deve apontar para o MÓDULO RESPONSÁVEL e explicar o relacionamento.

Exemplos:

- `aspnet-core` depende de CRITÉRIOS de `security`, `testing`, `architecture` e `devops`.
- `database` depende de `security`, `architecture` e `devops`.
- `ui` e `flutter` compartilham principios de EXPERIÊNCIA, acessibilidade e consistencia visual.
- `ai` depende de SEGURANÇA, privacidade, AVALIAÇÃO e rastreabilidade.

## Governanca arquitetural

MUDANÇAS que alteram estrutura, contrato de MÓDULO, obrigatoriedade de artefatos ou CRITÉRIOS globais devem ser tratadas como MUDANÇAS arquiteturais do framework. Elas exigem justificativa, ATUALIZAÇÃO do changelog e, quando apropriado, registro de DECISÃO.
