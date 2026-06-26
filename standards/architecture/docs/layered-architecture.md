# Arquitetura em Camadas

## Objetivo

A arquitetura em camadas organiza responsabilidades por níveis, reduzindo mistura entre apresentação, aplicação, domínio e infraestrutura.

## Camadas recomendadas

### Apresentação

Responsável por entrada e saída: APIs, interfaces, páginas, controllers, endpoints ou adaptadores de comunicação.

### Aplicação

Orquestra casos de uso, valida permissões, coordena transações e chama serviços de domínio ou portas de infraestrutura.

### Domínio

Contém regras de negócio, entidades, objetos de valor, políticas, eventos de domínio e invariantes.

### Infraestrutura

Implementa persistência, serviços externos, mensageria, arquivos, cache, e-mail e integrações técnicas.

## Regra de dependência

Camadas externas podem depender de camadas internas, mas camadas internas não devem depender de detalhes externos. O domínio deve ser o núcleo mais estável.

## Quando usar

Use quando o sistema tem regras de negócio relevantes e precisa separar responsabilidades para facilitar manutenção e testes.

## Cuidados

- Evite camadas artificiais sem responsabilidade real.
- Evite transformar a camada de aplicação em uma coleção de repasses sem valor.
- Evite colocar regra de negócio em repositórios, controllers ou componentes visuais.

## Exemplo conceitual

```text
Presentation -> Application -> Domain
             -> Infrastructure
```

A infraestrutura deve implementar contratos consumidos pela aplicação, sem contaminar o domínio com detalhes técnicos.
