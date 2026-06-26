# Guia de Contribuicao

Obrigado por contribuir com o Veltis Standards. Este repositorio define padroes que podem influenciar multiplos projetos, por isso cada alteracao deve ser clara, justificavel e facil de revisar.

## Principios de contribuicao

- Prefira conteudo objetivo, aplicavel e reutilizavel.
- Explique o motivo da mudanca, nao apenas o texto alterado.
- Evite criar padroes baseados em um unico projeto sem indicar contexto e limites.
- Preserve consistencia de nomenclatura, estrutura e tom entre os modulos.
- Registre excecoes e decisoes relevantes em documentos apropriados.
- Nao misture conteudo deste framework com documentacao de produtos especificos, incluindo Veltis AI Platform.

## Fluxo recomendado

1. Abra uma branch com nome descritivo, por exemplo `docs/security-baseline` ou `standards/git-pr-template`.
2. Atualize apenas os modulos ou documentos relacionados ao objetivo da mudanca.
3. Revise links, titulos, listas e exemplos antes de abrir pull request.
4. Atualize o `CHANGELOG.md` global quando a mudanca afetar o framework como um todo.
5. Atualize o `CHANGELOG.md` do modulo quando a mudanca for especifica de um modulo.
6. Solicite revisao de pessoas que conhecam o dominio afetado.

## Criterios para aceitar mudancas

- O conteudo resolve uma necessidade real de engenharia, produto ou operacao.
- O texto e claro para pessoas que nao participaram da discussao original.
- O padrao descreve quando deve ser usado e quando pode nao ser adequado.
- Exemplos, quando incluidos, sao genericos e nao expoem informacoes sensiveis.
- A mudanca nao cria conflito com padroes existentes sem explicar a substituicao.
- A estrutura do repositorio e dos modulos permanece consistente.

## Estilo de escrita

Use Markdown simples, frases diretas e titulos descritivos. Evite linguagem vaga como "boas praticas" sem dizer qual comportamento esperado. Mantenha nomes tecnicos em ingles quando forem convencoes da tecnologia.

## Conteudos proibidos

Nao inclua segredos, tokens, credenciais, dados reais de clientes, codigo-fonte de produtos, documentacao operacional sensivel ou conteudo especifico da Veltis AI Platform que nao seja um padrao reutilizavel.

## Versoes e releases

Mudancas que alteram criterios, obrigatoriedades ou fluxos de revisao devem ser destacadas no changelog e, quando necessario, acompanhadas de plano de migracao.
