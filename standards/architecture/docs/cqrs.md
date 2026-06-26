# CQRS

## Objetivo

CQRS separa operações de escrita e leitura quando elas possuem necessidades, modelos ou requisitos diferentes.

## Conceito

- Commands alteram estado.
- Queries consultam dados.

A separação pode ser apenas conceitual no código ou pode envolver modelos, bancos ou pipelines distintos em sistemas mais complexos.

## Quando usar

Use CQRS quando:

- leituras e escritas têm modelos muito diferentes;
- consultas exigem projeções específicas;
- regras de escrita precisam de validação forte;
- a complexidade do domínio justifica separar intenções.

## Quando evitar

Evite CQRS quando o CRUD simples atende bem. Separação excessiva pode aumentar complexidade sem benefício real.

## Práticas recomendadas

- Commands devem representar intenção de mudança.
- Queries não devem alterar estado.
- Handlers devem ser pequenos e testáveis.
- Validações de negócio devem permanecer explícitas.
- Eventos podem ser usados para atualizar projeções quando necessário.

## Exemplo conceitual

```text
CreateOrderCommand -> Handler -> Domain -> Repository
GetOrderSummaryQuery -> Handler -> Read Model
```

## Riscos

- Duplicação de modelos sem necessidade.
- Consistência eventual não explicada.
- Handlers com responsabilidades excessivas.
