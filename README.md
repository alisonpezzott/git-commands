# Power BI, Git, GitHub e VS Code

## Criação de conta  no GitHub  

Crie sua conta gratuita em https://github.com 

## Ferramentas para instalar

**Git**  
Ferramenta de versionamento de código local
Download: https://git-scm.com/downloads

**GitHub Desktop**  
Software para operação do GitHub com menos comandos
Download: https://desktop.github.com/download/

**GitHub CLI**  
Complemento para controlar o repositório GitHub pelo VSCode  
Download: https://cli.github.com/

**Visual Studio Code(VSCode)**  
Download: Microsoft Store ou https://code.visualstudio.com/  

**Power BI Desktop**  
Download: Microsoft Store ou https://apps.microsoft.com/detail/9ntxr16hnw1t?hl=pt-br&gl=BR  

### Comandos git  
`git init`
Inicia o repositório na pasta  

`git branch`
Mostra a lista de branches e indica em qual branch você está atualmente

`git branch -a`
Mostra todas as branches, incluindo as branches remotas

`git checkout -b <nome-da-branch>`
Cria e muda para uma nova branch chamada `<nome-da-branch>`

`git add .`  
Adiciona todos os arquivos modificados para o próximo commit

`git log`
Mostra o histórico de commits  

`git remote -v`
Mostra os repositórios remotos vinculados ao repositório local

`git remote add origin <url-do-repositorio-remoto>`
Linka o repositório local com o repositório remoto

`git commit -m "mensagem"`
Faz o commit das mudanças adicionadas com a mensagem "mensagem"  

`git push`
Envia as mudanças do repositório local para o repositório remoto

`git status`
Mostra o status do repositório

`git merge <nome-da-branch>`
Faz merge da branch `<nome-da-branch>` na branch atual

`git pull`
Atualiza o repositório local com as mudanças do repositório remoto

`git clone <url-do-repositorio-remoto>`
Clona o repositório remoto para o repositório local

`git push origin --delete <nome-da-branch>`
Deleta a branch `<nome-da-branch>` do repositório remoto

`git branch -d <nome-da-branch>`
Deleta a branch `<nome-da-branch>` do repositório local

`git pull origin <nome-da-branch>`
Atualiza a branch `<nome-da-branch>` do repositório local com a branch remota

`git push origin <nome-da-branch>`
Envia a branch `<nome-da-branch>` do repositório local para o repositório remoto

`git config --global user.email`

`gh repo create <nome-do-repositorio> --public`  
Cria um novo repositório no GitHub  

`gh repo delete <nome-do-repositorio>`  
Exclui o repositório `<nome-do-repositorio>` do GitHub

`gh auth refresh -h github.com -s delete_repo`
Exclui o repositório `<nome-do-repositorio>` do GitHub  

`gh repo delete <nome-do-repositorio>`  

### Erro HTTP 403: Permissões de Administrador Necessárias

Se você encontrar o erro `HTTP 403: Must have admin rights to Repository` ao tentar excluir um repositório no GitHub, siga os passos abaixo para resolver o problema:

    Este erro também pode ocorrer se você não tiver o escopo `delete_repo` autorizado. Para solicitar este escopo, execute o comando:
    `gh auth refresh -h github.com -s delete_repo`  