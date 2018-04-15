![enter image description here](http://capitalcode.com.br/curso-proj/1_2.jpg)![
](http://capitalcode.com.br/curso-proj/2.jpg)
![
](http://capitalcode.com.br/curso-proj/3.jpg)
![
](http://capitalcode.com.br/curso-proj/4.jpg)
![
](http://capitalcode.com.br/curso-proj/5.jpg)
![
](http://capitalcode.com.br/curso-proj/6.jpg)
![
](http://capitalcode.com.br/curso-proj/7.jpg)
![
](http://capitalcode.com.br/curso-proj/8.jpg)
![
](http://capitalcode.com.br/curso-proj/9.jpg)
![
](http://capitalcode.com.br/curso-proj/10.jpg)
![
](http://capitalcode.com.br/curso-proj/11.jpg)

## Guia Prático de introdução ao Git e Github

 -  [**Configurando Usuário Global**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#configurando-usu%C3%A1rio-global)
 - [**Configurando E-mail Global**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#configurando-e-mail-global)
 - [**Criando Repositório Local**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#criando-reposit%C3%B3rio-local)
 - [**Visualizando Status de nosso repositório**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#criando-reposit%C3%B3rio-local)
- [**Adicionando arquivos do Working Directory para a Staging Area**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#visualizando-status-de-nosso-reposit%C3%B3rio)
- [**Adicionando arquivos da Staging Area para o Git Directory**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#adicionando-arquivos-do-working-directory-para-a-staging-area)
- [**Alterando Mensagem de um Commit**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#alterando-mensagem-de-um-commit)
- [**Saindo de Arquivo "VIM"**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#saindo-de-arquivo-vim)
- [**Tags no Git**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#tags-no-git)
- [**Listar Tag**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#listar-tag)
- [**Listando Todos os Commits Realizados**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#listando-todos-os-commits-realizados)
- [**Criando Tag em Commit Existente**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#criando-tag-em-commit-existente)
- [**Acessando Tags de Versões Anteriores**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#acessando-tags-de-versões-anteriores)
-  [**Como Deletar uma Tag**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#como-deletar-uma-tag)
-  [**Branch**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#branch)
-  [**Listando Branch**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#listando-branch)
-  [**Criando Branch**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#criando-branch)
- [**Alternando entre Branches**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#alternando-entre-branches)
-  [**Merge entre Branches**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#merge-entre-branches)
-  [**Deletando Branch**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#deletando-branch)
-  [**Ambiente Gráfico do Git**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#ambiente-gráfico-do-git)
-  [**Gerando Chave ssh para acesso direto ao Github com o Git**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#gerando-chave-ssh-para-acesso-direto-ao-github-com-o-git)
-  [**Git Push**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#git-push)
-  [**Clonando Repositório do Github para o Git**](https://github.com/Capitalcode/Curso-Github/blob/master/README.md#clonando-repositório-do-github-para-o-git)

## Configurando Usuário Global

    git config --global user.name "Capital Code"
   

## Configurando E-mail Global

    git config --global user.email "cursos@capitalcode.com.br"

## Criando repositório Local

Primeiramente, crie um repositório no seu explorador de arquivos e entre neste repositório com o git, o nome do nosso repositório e "Local":

    cd local
    git init

## Visualizando Status de nosso repositório

    git status

## Adicionando arquivos do Working Directory para a Staging Area

    git add local/
    or
    git add . 

## Adicionando arquivos da Staging Area para o Git Directory

    git commit -m "Meu Primeiro Commit"


 ## Alterando Mensagem de um Commit

    git rebase -i --root

## Saindo de Arquivo "VIM"

    :wq
    //Salva e sai do VIM

## Tags no Git

Tags são "apelidos" para índices no Git, dessa forma podemos transitar entre versões:

## Listar Tag

    git tag

## Criar Tag

    git tag -a v1.0 -m "Versão 1.0"

## Listando Todos os Commits Realizados

    git log --pretty=oneline

## Criando Tag em Commit Existente

    git tag -a v1.2 521747298a3790fde1710f3aa2d03b55020575aa -m "Versão 1.2"

## Acessando Tags de Versões Anteriores

    git checkout v1.0

## Como Deletar uma Tag

Volte para o Branch Master 

    git checkout master

Delete a Tag

    git tag -d v1.0

   ## Branch

Um branch no Git é simplesmente um leve ponteiro móvel que aponta para o commit. O nome do branch padrão no Git é master. Como você inicialmente fez commits, você tem um branch principal (`master branch`) que aponta para o último commit que você fez. Cada vez que você faz um commit ele avança automaticamente.

## Listando Branch

    git branch

## Criando Branch

    git branch teste

Acabamos de criar um ambiente de teste

   ## Alternando entre Branches

    git checkout teste

## Merge entre Branches

Volte para o Branch master

    git checkout master

Agora faça o Merge (Junção entre os novos arquivos na Branch de teste e a Branch Master)

    git merge teste

## Deletando Branch

    git branch -d teste

## Ambiente Gráfico do Git

    gitk
    
## Gerando Chave ssh para acesso direto ao Github com o Git

    ssh-keygen

## Git Push

    git push https://github.com/Capitalcode/Curso-Github.git

## Clonando Repositório do Github para o Git

    git clone https://github.com/Capitalcode/Curso-Github.git



 

