# Sincronização Entre Máquinas

## Objetivo

Orientar o trabalho em múltiplas máquinas sem perda de alterações, divergência de branches ou publicação acidental de arquivos locais.

## Princípio

O repositório remoto deve ser a fonte de sincronização. Mudanças relevantes devem ser commitadas e enviadas para uma branch remota antes de trocar de máquina.

## Encerrar trabalho em uma máquina

```bash
git status
git add caminho/do/arquivo.md
git commit -m "docs: update git workflow guide"
git push origin nome-da-branch
```

Se a mudança ainda não estiver pronta para commit, prefira criar um commit temporário claro em branch própria, evitando stash como mecanismo de longo prazo.

## Retomar em outra máquina

```bash
git fetch origin
git switch nome-da-branch
git pull origin nome-da-branch
```

Se a branch ainda não existe localmente:

```bash
git switch -c nome-da-branch origin/nome-da-branch
```

## Uso de stash

Use stash apenas para mudanças temporárias e locais:

```bash
git stash push -m "wip ajustes documentação git"
git stash list
git stash pop
```

Não use stash como substituto de commit para trabalho importante.

## Cuidados

- Configure o mesmo nome e e-mail Git nas máquinas autorizadas.
- Não copie `.git` manualmente entre diretórios.
- Não versionar arquivos de configuração pessoal.
- Sempre rode `git status` antes de trocar de branch.
- Evite trabalhar na mesma branch em duas máquinas sem push e pull frequentes.

## Recuperação

Para verificar commits locais não enviados:

```bash
git log --oneline origin/nome-da-branch..HEAD
```

Para verificar commits remotos ainda não trazidos:

```bash
git log --oneline HEAD..origin/nome-da-branch
```
