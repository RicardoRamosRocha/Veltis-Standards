# Template de Mensagem de Commit

## Formato

```text
tipo(escopo opcional): descrição objetiva

Contexto adicional opcional.
```

## Tipos recomendados

- `feat`: nova funcionalidade.
- `fix`: correção.
- `docs`: documentação.
- `refactor`: reestruturação sem mudança funcional.
- `test`: testes.
- `chore`: manutenção.
- `ci`: integração contínua.
- `security`: segurança.

## Exemplos

```bash
git commit -m "docs(git): add branch naming rules"
git commit -m "fix(auth): validate expired session"
git commit -m "security(api): restrict admin endpoint access"
```

## Checklist

- [ ] A mensagem explica a intenção da mudança.
- [ ] O tipo está correto.
- [ ] O escopo é útil quando usado.
- [ ] O commit não mistura assuntos independentes.
- [ ] O commit não contém segredos ou dados sensíveis.
