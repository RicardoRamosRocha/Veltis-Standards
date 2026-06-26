# Organizacao

## Estrutura de pastas

O repositorio usa uma organizacao simples e previsivel:

```text
assets/
case-studies/
docs/
examples/
standards/
templates/
```

A pasta `docs/` contem a documentacao central do framework. A pasta `standards/` contem os modulos tematicos. As demais pastas em nivel global armazenam recursos compartilhados.

## Nomenclatura

- Use nomes de pastas em minusculo e com hifen quando houver mais de uma palavra.
- Use nomes de arquivos descritivos em Markdown.
- Preserve os arquivos obrigatorios dos modulos com os nomes definidos: `README.md`, `MANIFEST.md`, `CHANGELOG.md`, `roadmap.md` e `backlog.md`.
- Evite abreviacoes que nao sejam amplamente reconhecidas.

## Responsabilidades dos arquivos principais

### README.md

Apresenta o proposito, escopo, forma de uso e principios do repositorio ou modulo.

### MANIFEST.md

Define contrato, responsabilidade, artefatos esperados, criterios de qualidade e governanca.

### CHANGELOG.md

Registra mudancas relevantes, com foco em rastreabilidade e impacto.

### roadmap.md

Organiza a evolucao planejada em fases ou marcos.

### backlog.md

Mantem itens pendentes, melhorias e necessidades identificadas para refinamento futuro.

## Regras de manutencao

- Atualize documentos proximos ao contexto da mudanca.
- Quando uma mudanca afetar varios modulos, registre tambem o impacto no nivel global.
- Nao duplique conteudo entre modulos; use referencias cruzadas quando necessario.
- Mantenha exemplos genericos e sem dados sensiveis.
- Revise periodicamente itens de backlog para remover obsolescencia.

## Separacao de conteudo

O Veltis Standards deve conter padroes reutilizaveis. Documentos de produtos, decisoes especificas de clientes ou detalhes de implementacao proprietaria devem permanecer em seus respectivos repositorios.
