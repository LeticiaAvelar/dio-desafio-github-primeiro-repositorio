Link Para Download: https://central.github.com/deployments/desktop/desktop/latest/win32

O Git Bash é um terminal estendido para otimizar o uso do GitHub.



## Comandos Básicos

- control + L = limpar tela
- mkdir = criar diretório (pasta) dentro do local
- rm -d + nome do diretório = vai remover uma pasta **VAZIA** 
  *(importante colocar o nome da pasta, para que ele entenda que não é apenas um arquivo)*
- rm -r + nome do diretório = vai remover uma pasta **COM ARQUIVOS** 
  *(importante colocar o nome da pasta, para que ele entenda que não é apenas um arquivo)*
- ls = listar o que tem dentro da pasta
- cd + *algo* = ir para pasta *x* *(exemplo: cd c/users/letic/)*
- cd .. = retroceder um nível *(voltar para a pasta anterior)*
- pwd = aparece todo o caminho tomado até chegar na pasta/arquivo atual
- -a = mostrar arquivos ocultos
- mv + *nome* + ./ *pasta* = mover arquivo para *X* pasta
- echo > (nome.extensão, *por exemplo README.md*) = criar arquivo
- git status = mostra a situação do arquivo, modificações feitas etc
- ls -a = mostra arquivos ocultos
- up = volta um comando
- down = avança um comando
- tab = autocompleta o nome do arquivo ou pasta
- control + A = vai para o início da linha
- control + E = vai para o fim da linha
- control + setas laterais (<- | ->) = pula uma palavra para esquerda ou direita, respectivamente

Arquivos markdown usam o formato de extenção ".md"

Dicas para usar o typora = ajuda(h) > markdown reference



## Passo a passo para mandar arquivos do PC > GitHub

1. Faça as modificações necessárias *(alterar arquivos, editar, criar novos textos etc)*
2. Dê um git bash no local onde foram feitas as alterações ou faça o caminho manualmente através dos comandos
3. git status *(para verificar se ele reconheceu que houveram mudanças)*
4. git add . *(para incluir todas as alterações feitas, caso deseja apenas em um arquivo específico deve-se digitar "git add "nome do arquivo.extensão")*
5. git status
6. git commit -m "*INSIRA AQUI O QUE FOI FEITO DE ALTERAÇÃO/COMENTARIOS*"
7. git status
8. git push origin main *(ou master, de acordo com sua máquina)*



#### Para modificações feitas diretamente no repositório remoto do Git Hub, para que seja reconhecido no repositório do PC/Bash, é preciso dar um "git pull" dentro do git bash.
