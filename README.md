# projeto-barbearia
Projeto barbearia feito em node e react

# Criando aplicação node com yarn
  
  1) Segue abaixo os comandos da criação do backend.
     comando: mkdir prjeto
     comando: cd prjeto
     comando: yarn init -y 
     comentário: Esse comando cria um arquivo package.json dentro da pasta prjeto. 
  
  2) Segue abaixo o comando para instalar as bibliotecas sucrase, nodemon em modulo desenvolvimento. 
        comando:    yarn add sucrase nodemon -D   
     comentário: Sucrase serve para podermos usar o import no node.
     comentário: nodemon server para qualquer alteração no codigo o sistema se atualiza.
     
 3) Iremos instalar express um dependência. 
    comando: yarn add express 
    comentários: Quando você instalar o express a instalção irá adicionar no arquivo package.json algunas anotações, com essa abaixo: 
       "dependencies": {
       "express": "^4.17.1"
    }
4) Nesse item iremos criar uma pasta src e dentro dela três arquivos, app.js, routes.js e sever.js.
     O arquivo app.js é onde vai ficar configurado o servidor express 
     O arquivo routes já fala por se só, arquivo onde ficará as rotas  
     O arquivo sever.js onde iremos chamar a aplicação na porta especifica 
     
5) Iremos criar um arquivo nodemn.json para funcionar sucrase e configuração no package.json
   consfiguração do package.json
    "scripts" {
               "dev": "nodemon src/server.js",
               "dev:debug": "nodemon --inspect src/server.js" 
               }
   Configuração do arquivo nodemon.json
       {
        "execMap":{
               "js": "node -a sucrase/register"
                 }
       }
               
     
   
      
