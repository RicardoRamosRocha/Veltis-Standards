# Documentação de API

## Visão geral

Descreva o propósito da API, consumidores esperados e responsabilidades principais.

## Autenticação

Explique o mecanismo de autenticação e requisitos de autorização.

## Convenções

- Formato de payload: JSON.
- Datas: ISO 8601.
- Erros: estrutura padronizada.

## Endpoints

### Método /recurso

Descrição do endpoint.

Parâmetros:

| Nome | Tipo | Obrigatório | Descrição |
| --- | --- | --- | --- |
| id | string | Sim | Identificador do recurso |

Resposta de sucesso:

```json
{
  "id": "exemplo"
}
```

Erros esperados:

- `400`: requisição inválida.
- `401`: autenticação ausente ou inválida.
- `403`: acesso negado.
- `404`: recurso não encontrado.

## Versionamento

Explique a estratégia de versionamento da API.
