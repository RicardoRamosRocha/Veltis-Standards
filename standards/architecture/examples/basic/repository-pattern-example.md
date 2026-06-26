# Exemplo - Repository Pattern

## Cenário

Um caso de uso precisa carregar um agregado de cliente e persistir alterações após validações.

## Modelo conceitual

```text
Caso de uso -> Contrato de repositório -> Implementação de infraestrutura -> Banco de dados
```

## Boa aplicação

O repositório oferece operações com significado para o domínio, como recuperar um cliente por identificador ou salvar um agregado validado.

## Má aplicação

Um repositório que apenas expõe operações genéricas do ORM sem agregar intenção tende a aumentar abstração sem benefício.
