# Exemplo - Monólito Modular

## Cenário

Sistema SaaS com módulos de identidade, faturamento e catálogo.

## Estrutura conceitual

```text
Modules/
  Identity/
  Billing/
  Catalog/
Shared/
```

## Regras

- Identity controla usuários, perfis e autenticação.
- Billing controla planos, cobranças e faturas.
- Catalog controla produtos ou recursos disponíveis.
- Módulos não acessam dados internos uns dos outros sem contrato.

## Benefício

O sistema mantém implantação simples, mas preserva fronteiras que podem evoluir futuramente.
