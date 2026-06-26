# Guia de CONTRIBUIÇÃO

Obrigado por contribuir com o Veltis Standards. Este REPOSITÓRIO define PADRÕES que podem influenciar multiplos projetos, por isso cada ALTERAÇÃO deve ser clara, justificavel e FÁCIL de revisar.

## Principios de CONTRIBUIÇÃO

- Prefira CONTEÚDO objetivo, APLICÁVEL e reutilizavel.
- Explique o motivo da MUDANÇA, NÃO apenas o texto alterado.
- Evite criar PADRÕES baseados em um ÚNICO projeto sem indicar contexto e limites.
- Preserve consistencia de nomenclatura, estrutura e tom entre os MÓDULOS.
- Registre EXCEÇÕES e DECISÕES relevantes em documentos apropriados.
- NÃO misture CONTEÚDO deste framework com DOCUMENTAÇÃO de produtos especificos, incluindo Veltis AI Platform.

## Fluxo recomendado

1. Abra uma branch com nome descritivo, por exemplo `docs/security-baseline` ou `standards/git-pr-template`.
2. Atualize apenas os MÓDULOS ou documentos relacionados ao objetivo da MUDANÇA.
3. Revise links, titulos, listas e exemplos antes de abrir pull request.
4. Atualize o `CHANGELOG.md` global quando a MUDANÇA afetar o framework como um todo.
5. Atualize o `CHANGELOG.md` do MÓDULO quando a MUDANÇA for ESPECÍFICA de um MÓDULO.
6. Solicite REVISÃO de pessoas que conhecam o DOMÍNIO afetado.

## CRITÉRIOS para aceitar MUDANÇAS

- O CONTEÚDO resolve uma necessidade real de engenharia, produto ou OPERAÇÃO.
- O texto e claro para pessoas que NÃO participaram da discussao original.
- O PADRÃO descreve quando deve ser usado e quando pode NÃO ser adequado.
- Exemplos, quando incluidos, SÃO GENÉRICOS e NÃO expoem INFORMAÇÕES sensiveis.
- A MUDANÇA NÃO cria conflito com PADRÕES existentes sem explicar a substituicao.
- A estrutura do REPOSITÓRIO e dos MÓDULOS permanece consistente.

## Estilo de escrita

Use Markdown simples, frases diretas e titulos descritivos. Evite linguagem vaga como "boas PRÁTICAS" sem dizer qual comportamento esperado. Mantenha nomes TÉCNICOS em ingles quando forem convencoes da tecnologia.

## CONTEÚDOS proibidos

NÃO inclua segredos, tokens, credenciais, dados reais de clientes, codigo-fonte de produtos, DOCUMENTAÇÃO operacional sensivel ou CONTEÚDO especifico da Veltis AI Platform que NÃO seja um PADRÃO reutilizavel.

## VERSÕES e releases

MUDANÇAS que alteram CRITÉRIOS, obrigatoriedades ou fluxos de REVISÃO devem ser destacadas no changelog e, quando NECESSÁRIO, acompanhadas de plano de migracao.
