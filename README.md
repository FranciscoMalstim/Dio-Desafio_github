# Repositótio do Desafio de Projeto de Git/GitHub da Dio.

Desafio de Projeto Git/GitHub

## Segue alguns comando basicos para iniciar trabalhos com o Git/GitHub.

# Inicia o git
git init

# Adiciona todos os arquivos alterados
git add .

# Cria commit
## Padrões a se seguir de mensagem
### "Shore: para commits que não são fix e nem features"
### "Fix: para resolução de bugs"
### "Feature: para funcionalidades"
git commit -m "mensagem de commit"

# Subir branch
git push -u origin "nome da branch"

# Desfaz os dois ultimos commits
git rebase HEAD~2

# Cria branch
## Padrões de nome de branch
### "SHORE/(nome da branch)" - Quando não é fix e nem feature
### "FIX/(nome da branch)" - Quando é uma branch que irá resolver um bug
### "FEATURE/(nome da branch)" - Para novas funcionalidades
git checkout -b "nome da branch"

# Muda de branch
git checkout "nome da branch"

# Atualizar branch com a main
git pull origin main
# Atualizar branch main
git pull

# Apagar branch
git branch -D "nome da branch"

# Desfaz commit específico
## Primeiro pegue o hash do commit
git branch
## Após obter o hash
git reset --soft "hash do commit"

# Trocar mensagem de commit
## Após executar o comando será aberto o editor vim
git commit --amend

# Envia todos os arquivos alterados para a area de staging
## Isso é utilizado quando precisamos trabalhar em outra feature
git stash

# Restaura os arquivos do stash
git stash pop

# Mostra oque está no stash
git stash list

# Remove arquivo que está sendo monitorado pelo git
git rm --cached "nome do arquivo"


## Sobre merge de branch

Para dar merge em uma branch basta dar o seguinte comando


# Volta para a branch main
git checkout main

# Merge na branch
git merge "nome da branch a ser mergeada"


Recomendado para dar merge em uma branch, principalmente trabalhando em grupo é dar `push` na branch e criar uma `pull request` no github.
