# Manifesto do Modulo ASP.NET Core

## Identidade

- Modulo: $(System.Collections.Hashtable.S)
- Nome: ASP.NET Core
- Area: desenvolvimento backend com ASP.NET Core
- Status: inicial
- Responsabilidade: padronizar APIs, configuracao, injecao de dependencia, middlewares, autenticacao, validacao, logging, tratamento de erros e organizacao de projetos

## Contrato do modulo

Este modulo deve manter a estrutura padrao definida pelo Veltis Standards: README.md, MANIFEST.md, CHANGELOG.md, oadmap.md, acklog.md, docs/, 	emplates/, examples/, case-studies/, dr/, eleases/ e ssets/.

## Responsabilidades

- Definir criterios reutilizaveis para desenvolvimento backend com ASP.NET Core.
- Orientar equipes sobre quando e como aplicar o padrao.
- Manter templates e exemplos coerentes com a pratica recomendada.
- Registrar evolucao, decisoes e pendencias relevantes.
- Evitar dependencia de um produto especifico da Veltis.

## Entregaveis

Os principais entregaveis esperados sao: guias de API, templates de endpoints, convencoes de configuracao, criterios de observabilidade e exemplos de estrutura.

## Criterios de aceite para evolucao

Uma mudanca neste modulo deve preservar a estrutura obrigatoria, deixar claro o problema que resolve, indicar impacto em projetos existentes quando houver, atualizar changelog, roadmap ou backlog conforme necessario e manter consistencia com os demais modulos.

## Governanca

Alteracoes pequenas podem ser revisadas dentro do proprio modulo. Alteracoes que criem obrigatoriedade, alterem fluxo de trabalho, impactem seguranca ou afetem mais de um modulo devem receber revisao tecnica mais ampla.

## Qualidade esperada

O modulo deve favorecer APIs consistentes, contratos explicitos, erros previsiveis, seguranca aplicada e codigo testavel. Conteudos que nao ajudem uma decisao, revisao ou execucao devem ser simplificados, movidos para exemplos ou removidos.
