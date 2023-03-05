# Whatsapp-bot

## Primeiro crie a sua pasta com o nome do projeto
mkdir whatsapp-bot

Entre na pasta criada: 
cd whatsapp-bot

## Crie o arquivo package.json com o comando
npm init -y

Adicione ao seu package.json o “type” como “module” para podermos usar a sintaxe de import do ES6 Modules.

## Instale venom-bot como uma dependencia do seu projeto
npm install venom-bot

## Crie um arquivo principal
Crie um arquivo index.js na raiz do projeto

No nosso arquivo index iremos criar uma nova sessão e chamar nossa função start() após a conexão ser feita com sucesso. Para que a gente possa observar qualquer evento disparado de mensagem no nosso whatsapp iremos chamar a função onAnyMessage do client para que ele observe todas as mensagens enviadas incluindo as nossas, e passaremos como parametro uma function como callback para que seja executada sempre que uma nova mensagem for enviada, validaremos então o conteúdo da mensagem, se o conteúdo for “hello” iremos enviar uma mensagem de volta “🤖 world 🌎”.

(img1.png)

