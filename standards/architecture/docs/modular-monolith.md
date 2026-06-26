# Monólito Modular

## Objetivo

Monólito modular organiza um sistema em módulos internos bem delimitados, mantendo implantação única sem perder clareza de fronteiras.

## Quando usar

Use quando o produto precisa de evolução rápida, consistência transacional e simplicidade operacional, mas possui domínios ou capacidades que precisam ser isolados.

## Características

- Implantação única.
- Módulos com responsabilidades claras.
- Dependências internas controladas.
- Dados podem ser compartilhados fisicamente, mas devem ter ownership lógico.
- Comunicação entre módulos deve seguir contratos definidos.

## Fronteiras

Cada módulo deve possuir:

- objetivo claro;
- linguagem própria quando necessário;
- interfaces públicas internas;
- dados sob responsabilidade definida;
- testes e documentação do comportamento esperado.

## O que evitar

- Módulos que acessam diretamente dados internos de outros módulos.
- Dependências circulares.
- Pasta por tipo técnico em vez de capacidade de negócio quando o domínio pedir modularidade.
- Transformar o monólito modular em microsserviços sem necessidade operacional.

## Evolução

Um módulo bem isolado pode, no futuro, ser extraído para serviço separado se houver justificativa de escala, autonomia ou ciclo de vida.
