## Aula 08 | Trabalhando com Branches - Criando, Mesclando e Deletando

Branches são ramos dentro de um repositório. Nelas o desenvolvedor pode fazer testes e alterações do código sem que essas alterações afetem a branch main.

### Criar e trocar de uma branch para outra

Para mudar da branch atual para a branch desejada, deve-se utilizar o comando:

```
$ git checkout -b <NOME DA BRANCH>
```
Após fazer a troca de branchs todos os seus commits serão salvos na branch atual, enquanto a branch principal permanecerá sem alterações no arquivos.

Para retorna para a branch main, deve-se utilizar o comando:
```
$ git checkout main
```
Para saber o último commit de cada branch, deve-se utilizar o comando:
```
$ git branch -v
```
### Mesclando branchs
Para mesclar uma branch criada com a branch main, primeiro deve-se estar na branch main. Em seguida, utilize o comando:
```
$ git merge <NOME DA BRANCH QUE DESEJA MESCLAR COM A MAIN>
```
Isso fara com que todas as alterações feitas na branch criada sejam implementada na branch main.

### Deletando branchs
Após a mesclagem da branch criada com a branch main, não é mais necessário ter duas branchs com os mesmo arquivos. Pode-se excluir um branch utilizando o comando:
```
$ git branch -d <NOME DA BRANCH>
```
Para checar quais branchs existem no seu repositório, utilize o comando:
```
$ git branch
```