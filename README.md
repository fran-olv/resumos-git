# DIO | Resumos GIT
## Comandos do Git e Explicações 
 

```git clone``` clona o repositório remoto para o seu repositório local


```git pull``` atualiza o repositorio local, com as mudanças do repositório remoto.

```git add <nome do arquivo>``` adiciona um arquivo para área de preparação (staged) 

```git add .``` adiciona todos os arquivos que foram modificados para área de preparação


```git commit -m "descreva brevemente o que está alterando/criando"``` Cria o commit com a mensagem e arquivos que estão na área de preparação 

```git status``` Mostra modificações e arquivos que estão na area de preparação

> não aparecerem no git status: 
> - repositorios/pastas vazias novas 
> - arquivos listados no .gitignore não aparecerão no git status

```git log``` mostras os ultimos commits, mensagens e auto feitos no repositorios remoto e local

```git reflog``` mostra detalhadamente todos os commandos que foram executados, alguns não aparecem no git log. 


```git commit --amend -m "rescrevendo a ultima mensagem de commit"``` muda apenas a ultima msg de commit realizado. 

```git reset``` desfazer um commit (codifição tb). 
```git reset <nome do arquivo>``` retira o arquivo da area de preparação e o coloca na area de modificão (untracked)


- ```git reset --soft <hash do commit>``` arquivos que estavam posteriores ao commit indicado voltam para area de preparação (staged). \
- ```git reset --mixed <hash do commit>``` ou ```git reset <hash do commit>```  rquivos que estavam posteriores ao commit indicado voltam para area de modificão (untracked, antes do git add ). Mixed é opcional\
- ```git reset --hard <hash do commit> ``` ignora\deleta os arquivos do commit anterior e os desfaz.


> ```<hash do commit>``` pegar o penúltimo, e ai desfaz o último.


```git restore``` e ```git checkout -- .``` desfaz as alterações locais.

```git restore --stage <nome do arquivo``` retira o arquivo da área de preparação e o coloca na area de modificão (untracked)

```git remote add <url do repositorio remoto>``` conecta o repositório local com o remoto


```git push -u origin main``` envia o commit (msg+arquivos) para o repositorio remoto origin
