# Convenções de Nomenclatura Arquitetural

## Objetivo

Padronizar nomes arquiteturais para reduzir ambiguidade entre módulos, camadas, serviços, contratos e decisões.

## Princípios

- Nome deve refletir responsabilidade.
- Use termos do domínio quando existirem.
- Evite nomes genéricos como `Manager`, `Helper`, `Common` ou `Util` sem contexto forte.
- Preserve idioma técnico quando for convenção da tecnologia.

## Camadas

Nomes recomendados:

- `Domain`
- `Application`
- `Infrastructure`
- `Presentation`
- `Api`

## Casos de uso

Use nomes orientados a intenção:

```text
CreateCustomer
ApprovePayment
GenerateInvoice
```

## Serviços

Nomeie serviços pelo resultado ou responsabilidade:

```text
InvoiceCalculationService
AccessPolicyService
NotificationSender
```

## Repositórios

Use nomes ligados a agregados ou conceitos de persistência:

```text
CustomerRepository
InvoiceRepository
```

## ADRs

ADRs devem ser numerados e descritivos:

```text
ADR-001-layered-architecture.md
ADR-002-clean-architecture.md
```

## Revisão

Um nome arquitetural é bom quando reduz explicações, evita duplicidade e permanece válido mesmo com mudanças pequenas de implementação.
