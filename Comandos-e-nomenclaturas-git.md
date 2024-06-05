Comandos e nomenclaturas git (Baseados na aula de Git Udemy)

A maior parte do trabalho com git consiste em:
. Editar e salvar (git add)
. Commitar (git commit)
. Sincronizar com o repositório remoto (git push)

Staging area *é o conjuntos de arquivos cujas mudanças serão incluídas na nova versão*

# git config --global core.editor VIM   *Comando para trocar meu editor de texto padrão do git para VIM, melhor usar ele porque é mais leve que o VSCode*

# git status    *exibe as condições do diretório de trabalho e da área de Staging (indica arquivos não monitorados (untracked), modificados (modified), preparados (staged) e consolidados (commited).)* 

# git log   *escrito desta forma, sem argumentos, este comando lista os commits feitos neste repositório em ordem cronológica inversa*

# git init  *comando para que a pasta que estou no terminal, seja sincronizada com o git. Esse comando vai criar uma pasta oculta dentro desta pasta do terminal com o nome .git. Essa pasta .git armazena todas as configs que o git usa, mas não vou precisar acessar ela*

# git add <arquivo(s)>  *adiciona os novos arquivos e arquivos modificados para o próximo commit*
# git add .   *com o ponto, eu adiciono tudo que estiver no diretório atual no próximo commit, sem necessidade de digitar os nome dos arquivos 1 por 1*

# git commit  *salva o estado de um projeto no momento do comando git add(Caso não tenha parâmetro de mensagem, o commit vai abrir um editor de texto (eu escolhi o VIM) para escrever a mensagem)*
# git commit -m "colocar a mensagem aqui entre aspas"   *forma de já colocar a mensagem sem necessidade de abrir o editor de texto*

# git push *sincroniza o meu repositório local com o repositório remoto, ou seja, este comando vai enviar todos commits que ainda não tiverem sido enviados, para o repositório de origem*

# git diff  *exibe as diferenças entre commits e branchs*
# git diff [path]
# git diff HEAD~1   *HEAD~1 ou ~2 ou ~3... é como se fosse um apontador para o último commit da branch*