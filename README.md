# Comandos Git

> git clone

Serve para clonar um repositório da nuvem em uma pasta local da máquina, lembresse de usar o link após o comando. Exemplo:

```
git clone https://github.com/GabrielMoreto/Comandos_Git.git
```

> git log

Sereve para exibir os logs do repositório ou seja as alterações que foram feitas. Exemplo:

```
git log
```

> git log --oneline

Serve para exibir os logs de uma forma resumida.

```
git log --oneline
```

> git pull

Serve para atualizar o repositório caso você tenha feito alguma alteração no repositório na nuvem, para que essas alterações fiquem evidentes na pasta 
local da máquina você deve executar esse comando, lembresse de usar o link após o comando. Exemplo:

```
git pull https://github.com/GabrielMoreto/Comandos_Git.git
```

> git status

Serve para mostrar os arquivos que foram modificados. Exemplo:

```
git status https://github.com/GabrielMoreto/Comandos_Git.git
```

> git commit

Serve para fazer commits, você pode usar o nome do arquivo após o comando, para commitar somente ele, ou você também pode usar um ".", para commitar todos os arquivos
que modificou. Exemplo:

```
git commit README.md -m "Atualizando arquivo README.md"
```
```
git commit . -m "Atualizando arquivo README.md"
```

> git push

Serve para "empurrar" os arquivos para o GitHub, se você realizou alterações na pasta local, para que isso fique visível no GitHub utilize esse comando. Exemplo:

```
git push
```

> git restore --source

Serve para voltar em um determinado momento do código, fazer uma restauração, não se esqueça de colocar o hash do commit depois do comando se você colocar o nome do 
arquivo ele irá voltar apenas o arquivo especificado e se colocar um "." ele irá voltar todos os arquivos. Exemplo:

```
git restore --source b76bc86 .
```
```
git restore --source b76bc86 app.js"
```

> git add

Serve para adicionar as modificações ao repositório. Exemplo: 

```
git add contato.html
```
```
git add .
```

> git checkout

Serve para criar uma nova branch. Exemplo:

```
git checkout -b desenvolvimento
```

> git switch: 

Serve para alterar o branch atual. Exemplo:

```
git switch main
```
```
git switch desenvolvimento
```

> git branch

Serve para mostrar as branchs disponíveis e qual a branch que está ativa no momento. Exemplo: 

```
git switch desenvolvimento
```

> git merge

Serve para juntar as branchs, se fizer uma alteração na branch desenvolvimento ela não irá aparecer na branch main se você não executar esse comando. Exemplo:

```
git merge
```

