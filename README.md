# SI-projeto

## Manual de instalação

Fazer o download do Visual Studio Code para edição do código.
<https://code.visualstudio.com/>

Fazer download do Node.js versão LTS para rodar Javascript.
<https://nodejs.org/en/>

Fazer download do MySQL para rodar o banco de dados.
<https://dev.mysql.com/downloads/installer/>

Configuração do MySQL.
<https://www.youtube.com/watch?v=zpssr3u1EO8>

Com o Node.js e Visual Studio Code instalados, é necessário instalar o pacote Yarn e o Expo, para isso abra o terminal do Visual Studio Code e rode os seguintes comando.

```JavaScript
npm install yarn -g
npm install expo -g ou yarn add expo -g
```

Fazer o download do Git no computador para baixar o projeto do Github.
<https://git-scm.com/downloads>

Configuração do Git.
<https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Configura%C3%A7%C3%A3o-Inicial-do-Git>

Com o Git instalado, no terminal do Visual Studio Code rode o comando para fazer download do projeto.
git clone *link do repositório*

Com o repositório clonado, abra a pasta backend-si e dentro a pasta config o arquivo default.json e mude o nome da database, user e password que foi colocado quando configurado o MySQL.

## Como rodar o projeto

Com o terminal do Visual Studio Code aberto na pasta backend-si digite os seguintes comando para rodar.

```JavaScript
npm install // (deve ser rodado apenas uma vez ou quando tiver uma mudança nas dependências do projeto)

npm run tables // (deve ser rodado apenas uma vez ou quando tiver uma mudança nas tabelas do banco de dados)

npm run start
```

### Web

Com o terminal do Visual Studio Code aberto na pasta WEB_SI digite os seguintes comandos para rodar a aplicação.

```JavaScript
yarn // (deve ser rodado apenas uma vez ou quando tiver uma mudança nas dependências do projeto)

yarn dev
```

### Mobile

Fazer o download do ngrok para conseguir acessar o banco de dados no mobile.
<https://ngrok.com/download>

Com ngrok instalado, execute o arquivo ngrok.exe e rode o comando.

```JavaScript
ngrok http 4547 // (4547 é a porta utilizada pela equipe)
```

Esse comando vai gerar um link https, copie e cole no arquivo axios.ts localizado em mobile_si/src/api/axios.ts na linha baseURL.
foto de exemplo da função
baseURL: *link do ngrok ex: <https://example.ngrok.io>*

Com o terminal do Visual Studio Code aberto na pasta mobile_si digite os seguintes comandos para rodar a aplicação.

```JavaScript
yarn // (deve ser rodado apenas uma vez ou quando tiver uma mudança nas dependências do projeto)

yarn start ou expo start
```

Baixe o aplicativo em seu smartphone chamado *Expo Go*.

Aponte a câmera do celular para o QRCode que irá aparecer no terminal do Visual Studio Code que ao escanear abrirá o aplicativo em seu smartphone.
