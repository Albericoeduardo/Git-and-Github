## AULA 06 | Desfazendo alterações no repositório local

### Versionamento de diretório errado
Para remover o versionamento de um diretório foi iniciado sem intenção, é so remover a pasta .git que está no diretório. Podendo também ser usando o comando:
```
$ rm -rf .git
```
#### Restauração do arquivo para a versão anterior
```
$ git restore <NOME DO ARQUIVO>
```
#### Muda a mensagem do último commit para a mensagem desejada
```
# git commit --amend -m "Mensagem desejada"
```
#### Retorna os arquivo para o área staged:
```
$ git reset --soft <HASH DO COMMIT>
```
#### Retorna os arquivos para a área untracked:
```
$ git reset --mixed <HASH DO COMMIT>
```
#### Retorna os arquivos do commit e os apaga:
```
$ git reset --hard <HASH DO COMMIT>
```
