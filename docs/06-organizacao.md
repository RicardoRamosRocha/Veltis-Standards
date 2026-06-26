# ORGANIZAÇÃO

## Estrutura de pastas

O REPOSITÓRIO usa uma ORGANIZAÇÃO simples e previsivel:

```text
assets/
case-studies/
docs/
examples/
standards/
templates/
```

A pasta `docs/` contem a DOCUMENTAÇÃO central do framework. A pasta `standards/` contem os MÓDULOS tematicos. As demais pastas em NÍVEL global armazenam recursos compartilhados.

## Nomenclatura

- Use nomes de pastas em minusculo e com hifen quando houver mais de uma palavra.
- Use nomes de arquivos descritivos em Markdown.
- Preserve os arquivos obrigatorios dos MÓDULOS com os nomes definidos: `README.md`, `MANIFEST.md`, `CHANGELOG.md`, `roadmap.md` e `backlog.md`.
- Evite abreviacoes que NÃO sejam amplamente reconhecidas.

## Responsabilidades dos arquivos principais

### README.md

Apresenta o PROPÓSITO, escopo, forma de uso e principios do REPOSITÓRIO ou MÓDULO.

### MANIFEST.md

Define contrato, responsabilidade, artefatos esperados, CRITÉRIOS de qualidade e governanca.

### CHANGELOG.md

Registra MUDANÇAS relevantes, com foco em rastreabilidade e impacto.

### roadmap.md

Organiza a EVOLUÇÃO planejada em fases ou marcos.

### backlog.md

Mantem itens pendentes, melhorias e necessidades identificadas para refinamento futuro.

## Regras de MANUTENÇÃO

- Atualize documentos PRÓXIMOS ao contexto da MUDANÇA.
- Quando uma MUDANÇA afetar varios MÓDULOS, registre TAMBÉM o impacto no NÍVEL global.
- NÃO duplique CONTEÚDO entre MÓDULOS; use referencias cruzadas quando NECESSÁRIO.
- Mantenha exemplos GENÉRICOS e sem dados sensiveis.
- Revise periodicamente itens de backlog para remover obsolescencia.

## Separacao de CONTEÚDO

O Veltis Standards deve conter PADRÕES reutilizaveis. Documentos de produtos, DECISÕES ESPECÍFICAS de clientes ou detalhes de IMPLEMENTAÇÃO proprietaria devem permanecer em seus respectivos REPOSITÓRIOS.
