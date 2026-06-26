# ASP.NET Core Standard

## Proposito

O modulo ASP.NET Core define o padrao da Veltis para desenvolvimento backend com ASP.NET Core. Seu objetivo e padronizar APIs, configuracao, injecao de dependencia, middlewares, autenticacao, validacao, logging, tratamento de erros e organizacao de projetos.

Este modulo deve ser usado como referencia em novos projetos, revisoes tecnicas, evolucao de sistemas existentes e definicao de criterios de aceite relacionados ao tema.

## Escopo

O modulo cobre principios e criterios aplicaveis ao tema, responsabilidades minimas esperadas em projetos da Veltis, artefatos reutilizaveis para planejamento, execucao e revisao, exemplos e templates que reduzem ambiguidade, alem de registros de decisao e historico de evolucao do padrao.

## Fora de escopo

Este modulo nao deve conter codigo-fonte de produto, configuracoes sensiveis, dados reais de clientes ou documentacao operacional restrita. Conteudos especificos de um produto devem permanecer no repositorio do produto e apenas referenciar este padrao quando aplicavel.

## Artefatos esperados

- docs/: guias detalhados e referencias de uso.
- 	emplates/: modelos reutilizaveis.
- examples/: exemplos genericos e anonimizados.
- case-studies/: estudos de caso aplicaveis ao dominio.
- dr/: decisoes relevantes para evolucao do modulo.
- eleases/: notas de publicacao do modulo.
- ssets/: diagramas, imagens e materiais auxiliares.

## Como aplicar

1. Identifique se a entrega possui impacto em desenvolvimento backend com ASP.NET Core.
2. Consulte o manifesto do modulo para entender responsabilidades e criterios obrigatorios.
3. Use os templates disponiveis como ponto de partida.
4. Registre excecoes quando o projeto precisar divergir do padrao.
5. Atualize backlog, roadmap ou changelog quando uma melhoria no padrao for identificada.

## Criterios de qualidade

Um uso adequado deste modulo deve resultar em APIs consistentes, contratos explicitos, erros previsiveis, seguranca aplicada e codigo testavel.

## Relacionamentos

Este modulo pode se relacionar com outros padroes em standards/. Quando houver dependencia de outro dominio, prefira referenciar o modulo responsavel em vez de duplicar orientacoes.
