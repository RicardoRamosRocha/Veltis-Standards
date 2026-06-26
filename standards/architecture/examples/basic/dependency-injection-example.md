# Exemplo - Injeção de Dependência

## Cenário

Um caso de uso precisa enviar notificação após concluir uma operação.

## Desenho conceitual

```text
Caso de uso depende de NotificationSender.
Infrastructure fornece EmailNotificationSender.
```

## Benefício

O caso de uso não conhece detalhes de e-mail, provedor externo ou configuração. Em testes, a dependência pode ser substituída por implementação controlada.

## Cuidado

Se uma classe recebe dependências demais, revise a responsabilidade antes de adicionar novas abstrações.
