# Ciclo de Vida da Documentação

## Visão geral

A documentação deve evoluir junto com o projeto. Cada documento passa por criação, revisão, publicação, manutenção e eventual descontinuação.

## 1. Criação

Um documento deve ser criado quando houver uma necessidade real de alinhamento, registro ou execução. Antes de criar, verifique se já existe uma fonte oficial que possa ser atualizada.

Critérios para criação:

- existe público-alvo claro;
- existe uma pergunta ou decisão que o documento responde;
- o local do arquivo segue as convenções do projeto;
- o documento possui escopo definido.

## 2. Revisão

A revisão deve validar conteúdo, clareza, consistência, segurança e aderência ao padrão. Revisões relevantes devem acontecer em pull requests ou em processos equivalentes.

Critérios de revisão:

- o texto está em português e usa linguagem profissional;
- não há segredos, dados reais ou informação sensível;
- as seções obrigatórias estão presentes;
- links e referências são válidos;
- o documento não duplica informação sem necessidade.

## 3. Publicação

Um documento publicado deve representar a orientação vigente. Quando houver versões ou releases, a publicação deve estar associada a changelog ou release notes.

## 4. Manutenção

Documentos devem ser revisados quando houver mudança em requisitos, arquitetura, API, operação, segurança, processo ou versão. Documentos críticos devem ter revisão periódica definida.

## 5. Depreciação

Quando um documento deixar de ser aplicável, ele deve ser marcado como obsoleto, substituído por nova referência ou removido quando não houver necessidade histórica.

## 6. Arquivamento

Documentos com valor histórico podem ser mantidos em uma área de releases, ADRs ou arquivos de referência. O arquivamento deve deixar claro que o conteúdo não é mais a orientação vigente.

## Papéis recomendados

- Autor: cria ou atualiza o documento.
- Revisor técnico: valida precisão, impacto e consistência.
- Revisor de segurança: avalia riscos quando houver dados, acessos, infraestrutura ou integrações.
- Mantenedor: garante evolução e coerência ao longo do tempo.
