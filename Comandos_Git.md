# Comandos Git

> git clone

Serve para clonar um repositório da nuvem em uma pasta local da máquina, lembresse de usar o link após o comando e também 
de estar dentro da pasta onde você deseja que os arquivos fiquem. Exemplo:

```
git clone https://github.com/GabrielMoreto/Comandos_Git.git
```
Para mudar a pasta no cmd basta usar o comando "cd" seguido do caminho da pasta. no meu caso se eu utilizar o comando abaixo estarei dentro da pasta "Comandos_Git".

```
cd C:\Users\gabri\OneDrive\Área de Trabalho\Git\Git\Comandos_Git
```

> git log

Serve para exibir os logs do repositório ou seja as alterações que foram feitas. Exemplo:

```
git log
```

Vale lembrar que sempre ao final de uma alteração você deve fazer um commit, se você realizar uma alteração e não fizer o commit ela não ficará visível ao executar o comando.

> git log --oneline

Serve para exibir os logs de uma forma resumida, cada alteração irá aparecer em uma única linha. Exemplo:

```
git log --oneline
```

Vale lembrar que sempre ao final de uma alteração você deve fazer um commit, se você realizar uma alteração e não fizer o commit ela não ficará visível ao executar o comando.

> git pull

Serve para atualizar o repositório caso você tenha feito alguma alteração no repositório na nuvem, para que essas alterações fiquem evidentes na pasta 
local da máquina você deve executar esse comando, lembresse de usar o link após o comando. Exemplo:

```
git pull https://github.com/GabrielMoreto/Comandos_Git.git
```

> git status

Serve para mostrar os arquivos que foram modificados. Exemplo:

```
git status
```

> git commit

Serve para fazer commits, commits devem ser feitos sempre que você terminar de fazer uma alteração, os commits servem como uma espécie comentário para ajudar a entender o que foi feito. Você pode usar o nome do arquivo após o comando, para commitar somente ele, ou você também pode usar um ".", para commitar todos os arquivos
que modificou. Exemplo:

```
git commit README.md -m "Atualizando arquivo README.md"
```
Neste exemplo o arquivo "README.md" está especificado então o commit só sera feito para ele.

```
git commit . -m "Atualizando arquivo README.md"
```
Neste exemplo o . serve como parâmetro para commitar todos os arquivos. 

> git push

Serve para "empurrar" os arquivos para o GitHub, se você realizou alterações na pasta local, para que isso fique visível no GitHub utilize esse comando. Exemplo:

```
git push
```
Vale lembrar que você só irá conseguir utilizar esse comando caso tenha realizados os commits.

> git restore --source

Serve para voltar em um determinado momento do código ou seja para fazer uma restauração. Quando você executa o comando "git log --oneline" repare que na frente de cada log existe um código, esse código se chama hash, para que o comando funcione, você deve especificar o hash do momento que deseja restaurar. Exemplos:

```
git restore --source b76bc86 .
```
Neste exemplo foi utilizado o "." como parâmetro então todos os arquivos vão ser restaurados.

```
git restore --source b76bc86 app.js"
```
Neste exemplo foi especificado o arquivo "app.js", então somente ele será restaurado.

> git add

Serve para adicionar as modificações para o commit. Exemplo: 

```
git add contato.html
git commit -m "Atualizando arquivo contato.html"
```
Neste exemplo o arquivo "contato.html" foi adicionado, e para commitar ele basta apenas que eu execute o comando commit.


```
git add .
```
Neste exmplo eu adiciono todos os arquivos que tiveram alteração, quando eu realizar o commit ele irá ser feito para todos.

> git checkout

Serve para criar uma nova branch. Branchs são interessantes para criar ambientes como de desenvolvimento e produção. Exemplo:

```
git checkout -b desenvolvimento
```
Neste exemplo a branch desenvolvimento irá ser criada

> git switch: 

Serve para alterar o branch atual. Exemplo:

```
git switch prod
```
```
git switch dev
```

> git branch

Serve para mostrar as branchs disponíveis e qual a branch que está ativa no momento. Exemplo: 

```
git switch desenvolvimento
```

> git merge

Serve para juntar as branchs, se fizer uma alteração na branch desenvolvimento ela não irá aparecer na branch de produção se você não executar esse comando. Exemplo:

```
git merge
```