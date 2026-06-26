# Guia de Versionamento Documental

## Objetivo

Definir como documentos e módulos de documentação devem evoluir por versão, mantendo rastreabilidade e comunicação clara de mudanças.

## Quando versionar

Uma mudança deve ser versionada quando altera critérios, estrutura, obrigatoriedade, templates, processo de revisão ou orientação oficial usada por projetos.

Correções editoriais simples podem ser registradas apenas no histórico Git, desde que não alterem interpretação ou comportamento esperado.

## Versões do módulo

O módulo Documentation usa versões planejadas:

- `1.0`: fundação completa do padrão de documentação.
- `1.1`: expansão de templates e exemplos.
- `1.2`: refinamento com estudos de caso e automações de revisão.
- `2.0`: maturidade com governança avançada e indicadores.

## Changelog

O `CHANGELOG.md` deve registrar mudanças relevantes por versão. Cada entrada deve explicar o que foi adicionado, alterado, removido ou corrigido.

## Release notes

Release notes devem comunicar a versão para pessoas usuárias do padrão, destacando impacto, artefatos novos e orientações de adoção.

## Compatibilidade

Mudanças que quebram estrutura ou expectativa de uso devem ser destacadas. Quando possível, ofereça período de transição ou orientação de migração.

## Status

O arquivo `STATUS.md` deve indicar a versão vigente do módulo, seu estado, responsável e próximas entregas.
