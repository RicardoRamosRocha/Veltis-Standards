# Tags

## Objetivo

Definir como usar tags Git para marcar versões, releases e pontos relevantes de rastreabilidade.

## Convenção

Use tags semânticas com prefixo `v`:

```text
v1.0.0
v1.1.0
v1.1.1
```

Para pré-releases:

```text
v1.2.0-rc.1
v2.0.0-beta.1
```

## Criar tag

```bash
git switch main
git pull origin main
git tag -a v1.0.0 -m "Release v1.0.0"
git push origin v1.0.0
```

Use tags anotadas (`-a`) para releases formais porque elas carregam mensagem e metadados.

## Listar e inspecionar tags

```bash
git tag
git show v1.0.0
git log --oneline v1.0.0
```

## Remover tag criada por engano

```bash
git tag -d v1.0.0
git push origin --delete v1.0.0
```

Remover tag publicada deve ser exceção e precisa de alinhamento com a equipe.

## Relação com releases

Toda release formal deve ter tag correspondente. Release notes devem indicar a tag, data, mudanças relevantes e riscos conhecidos.

## O que evitar

- tags sem padrão, como `final`, `ok`, `deploy`;
- reutilizar tag para outro commit;
- criar tag sem changelog ou release notes quando houver impacto para usuários.
