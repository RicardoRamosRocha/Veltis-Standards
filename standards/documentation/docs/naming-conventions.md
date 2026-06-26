# Convenções de Nomenclatura

## Objetivo

Definir nomes previsíveis para arquivos e diretórios de documentação, facilitando localização, automação e revisão.

## Diretórios

- Use letras minúsculas.
- Use hífen para separar palavras.
- Evite acentos em nomes de arquivos e pastas.
- Use nomes no singular ou plural conforme o tipo de coleção já estabelecido no projeto.

Exemplos:

- `docs/`
- `templates/`
- `case-studies/`
- `release-notes/`

## Arquivos Markdown

- Use extensão `.md`.
- Use nomes descritivos.
- Use hífen entre palavras.
- Evite nomes genéricos fora de contextos padronizados.

Exemplos:

- `product-vision.md`
- `requirements.md`
- `architecture.md`
- `release-notes-template.md`

## Arquivos principais

Arquivos principais do repositório ou módulo devem manter nomes reconhecíveis:

- `README.md`
- `MANIFEST.md`
- `CHANGELOG.md`
- `STATUS.md`
- `roadmap.md`
- `backlog.md`

## ADRs

ADRs devem seguir numeração sequencial:

```text
ADR-001-titulo-da-decisao.md
ADR-002-titulo-da-decisao.md
```

## Releases

Notas de release devem indicar versão:

```text
v1.0.md
v1.1.md
v2.0.md
```

## Templates

Templates devem terminar com `-template.md` quando forem modelos copiáveis.

## Exemplos

Exemplos devem terminar com `-example.md` quando demonstrarem preenchimento de um template ou padrão.
