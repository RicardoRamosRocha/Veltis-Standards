# Guia de Documentação

## Objetivo

Este guia define como projetos da Veltis devem estruturar, escrever, revisar e manter documentação. Ele deve ser usado por equipes de produto, engenharia, arquitetura, qualidade, segurança e operação sempre que um projeto precisar registrar contexto, decisões, requisitos, APIs, módulos, processos ou releases.

A documentação deve reduzir ambiguidade, preservar memória técnica e permitir que uma pessoa nova no projeto consiga entender o essencial sem depender apenas de conversas informais.

## Documentação mínima por projeto

Todo projeto profissional da Veltis deve manter, no mínimo:

- `README.md`: visão geral, propósito, execução, estrutura e links importantes.
- visão de produto: problema, público, proposta de valor e objetivos.
- requisitos: requisitos funcionais, não funcionais, regras e critérios de aceite.
- backlog: épicos, histórias, prioridade, status e versão prevista.
- roadmap: evolução planejada por fases ou versões.
- arquitetura: contexto, decisões, componentes, integrações e riscos.
- changelog: histórico de mudanças relevantes.
- ADRs: decisões técnicas significativas e suas consequências.

## Níveis de documentação

### Estratégico

Explica por que o projeto existe, qual problema resolve e quais resultados espera alcançar. Deve ser compreensível por pessoas técnicas e não técnicas.

### Funcional

Descreve comportamentos, regras, fluxos, perfis, permissões e critérios de aceite. Deve apoiar análise, QA, desenvolvimento e validação de produto.

### Técnico

Registra arquitetura, APIs, dados, integrações, decisões, padrões de implementação, segurança, observabilidade e operação.

### Operacional

Explica como manter, publicar, monitorar, reverter ou diagnosticar o sistema. Deve ser objetivo, acionável e seguro.

## Critérios de qualidade

Uma documentação adequada deve ser:

- clara: usa linguagem direta e evita ambiguidade;
- útil: ajuda uma decisão, execução, revisão ou manutenção;
- atualizável: possui dono, data ou contexto de revisão;
- rastreável: conecta requisitos, decisões, mudanças e releases;
- segura: não expõe segredos, dados reais ou detalhes restritos;
- reutilizável: evita dependência desnecessária de um único projeto.

## Quando documentar

Documente quando uma informação for necessária para entender, operar, revisar ou evoluir o projeto. Mudanças relevantes em escopo, arquitetura, segurança, dados, APIs, dependências, integrações ou releases devem gerar atualização documental.

## Quando não documentar

Não documente ruído operacional passageiro, preferências pessoais sem impacto, detalhes que mudam a cada execução ou informações sensíveis que devem permanecer em sistemas internos controlados.

## Responsabilidade

A responsabilidade pela documentação é compartilhada. Quem propõe uma mudança deve atualizar os documentos afetados; quem revisa deve validar se a documentação continua suficiente para o próximo ciclo de manutenção.
