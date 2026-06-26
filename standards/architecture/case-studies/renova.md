# Estudo de Caso - Renova

## Contexto

Um sistema de CRM, atendimento, EAD e financeiro combina regras de domínio, dados pessoais e fluxos operacionais sensíveis. A arquitetura deve favorecer separação de responsabilidades e conformidade.

## Aplicação do padrão

- Usar camadas para separar apresentação, aplicação, domínio e infraestrutura.
- Proteger regras de acompanhamento, cursos e financeiro no domínio ou aplicação.
- Documentar decisões de dados pessoais, acesso e auditoria.
- Isolar integrações externas e persistência.

## Resultado esperado

Uma arquitetura mais testável, rastreável e preparada para evolução gradual, sem misturar regras de negócio com detalhes de UI ou banco.
