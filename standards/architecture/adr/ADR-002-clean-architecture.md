# ADR-002 - Usar Clean Architecture em domínios relevantes

## Status

Aceito

## Data

2026-06-26

## Contexto

Projetos com regras de negócio importantes precisam proteger domínio e casos de uso de detalhes técnicos como banco, UI e provedores externos.

## Decisão

Usar Clean Architecture quando o domínio, a testabilidade e a expectativa de evolução justificarem separação mais forte de dependências.

## Consequências

### Positivas

- Domínio menos acoplado a frameworks.
- Casos de uso mais testáveis.
- Troca de infraestrutura com menor impacto.

### Negativas

- Pode aumentar complexidade inicial.
- Exige cuidado para evitar abstrações sem valor.

## Critérios de revisão

Revisar se o custo estrutural superar os benefícios no contexto do projeto.
