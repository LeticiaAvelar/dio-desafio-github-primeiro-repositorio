# Resolvendo Conflitos :warning: ​​



### :point_right: ​Identificar arquivos com conflitos

- Use o comando **GIT STATUS** para visualizar.

O arquivo que aparecer em vermelho, é porque está conflitante _(provavelmente não mesclado -unmerged)_.

- Abra o arquivo que está com conflito _(exemplo: README.md)_

Ao abrir o arquivo, será possível visualizar alguns símbolos e escritos que indicam as alterações _(exemplo: <<<<<<< HEAD (sua versão local) ======= (versão remota) >>>>>>> (branch do remoto))_.

Também deve-se limpar a chave de commit que aparece (com letras e números). O arquivo deve estar limpo e sem marcas de conflito, sendo iguais remotamente e na sua máquina.

- Use o comando **GIT ADD "nome_do_arquivo"** _(exemplo: git add README.md)_
- Conclua a mesclagem do arquivo usando o comando GIT COMMIT -M "escreva qual foi o tipo de interação feita" _(exemplo: resolvendo conflitos no README.md)_
- Envie as alterações para o repositório remoto com o comando **GIT PUSH ORIGIN MASTER** _(ou MAIN, siga de acordo com a branch do seu pc)_

:red_circle:  Caso queira ou precise abortar a mesclagem, basta usar o comando **GIT MERGE --ABORT**



### :point_right: ​Enviar arquivos que estão na sua máquina para o repositório remoto

- Navegue até a pasta do repositório usando o comando **CD** _(exemplo:  cd /c/workspace/git dio/_, ou vá manualmente no local e dê um clique direito com o mouse e "Git Bash here"
- Verifique o status do repositório usando o comando **GIT STATUS**
- Adicione o arquivo ao índice *(staging area)*, usando o comando **GIT ADD "nome_do_arquivo.md"** ou **GIT ADD .** _(para vários arquivos -novos e modificados)_

Ao fazer isso, você está indicando ao git que deseja fazer a inclusão dessas alterações no próximo commit.

- Faça o commit para registrar a alteração com o comando **GIT COMMIT -M "escreva qual foi o tipo de alteração feita"**
- Por fim, envie as alterações para o repositório remoto no GitHub utilizando o comando **GIT PUSH ORIGIN MASTER** _(ou conforme sua branch)_.



### :point_right: ​Utilizando o comando GIT PULL

Ele é utilizado para atualizar sua cópia no repositório LOCAL (seu computador) com as alterações feitas no repositório REMOTO. Realiza o fetch *(baixa as alterações do remoto)* e o merge *(mescla essas alterações na sua branch atual)*.

- Navegue até a pasta do repositório usando o comando **CD** _(exemplo:  **cd /c/workspace/git dio/**)_, ou vá manualmente no local e dê um clique direito com o mouse e "Git Bash here"
- Verifique a branch atual com o comando **GIT BRANCH**
- Faça o pull para atualizar a branch com as mudanças usando o comando **GIT PULL ORIGIN MASTER** (ou a branch utilizada)