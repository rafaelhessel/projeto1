# projeto1
projeto para aprender a usar o github

# Anotações
git add

git add . - adiciona tudo

git init - inicializa

git status - status

git add - adiciona localmente

git commit -m "mensagem de mudança do codigo (commit inicial)" - commita localmente

git push --set-upstream origin (nome da branch, no caso master)master - primeiro push (coloca no github na master)

git push - segundo e outros pushs para o github

git reflog - ver as versoes dos commits

git reset --hard (colocar o codigo do commit que mostrou no git reflog) - serve para voltar para as versões do commit anteriores 

------------

para configurar o git 

 git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

git remote add origin "link do repositorio"

-------------------

BRANCH

galhos do codigo, ramificações

a branch padrão eh a master 

pensa como se fossem varios galhos, que contem varios frutos em cada galho, sendo cada fruto uma versão do codigo

geralmente em uma equipe, cada funcinario tem uma branch especifica 

no final eh feito um merge para juntar as diferentes branchs em um codigo unico 

git branch - mostra as branchs disponiveis 

git branch (nome da branch) - adiciona nova branch

git checkout (nome da branch) - muda a branch para que o codigo esta indo 

git pull - fazer antes de fazer o merge, para puxar atualizações do servidor para a maquina local

git merge (nome da branch que o codigo vai ser copiado, no caso staging) - fazer isso depois de fazer "git pull" fazer o merge de onde voce quer puxar o codigo, lembrando que vc tem que estar dentro da branch que voce quer, no caso ja estou dentro da master

---------------------

MERGE 

1. git pull da branch principal
2. gerar nova branch a partir da brnach principal
3. trabalhar e adicionar novas funcionalidades na nova branch que criou
4. finalizar o trabalho na branch temporaria 
5. git checkout na branch principal
6. git pull
7. mergiar o codigo da branch temporario com a branch principal(depois de testar)
8. git push da branch principal

para fazer alterações, primeiro voce cria o codigo em uma branch secundaria.
depois de testar o codigo, voce faz o merge

---------------

touch .gitignore - cria arquivo txt ignore

no arquivo ignore voce coloca os arquivos que vao ser desconsiderados do commit

tem que dar git add no arquivo git ignore


