<h1 align="center">
  <img style="background-color: #312e38; border-radius: 10px;" alt="gobarber-logo" src="https://user-images.githubusercontent.com/18368947/87232012-1bf67680-c392-11ea-9f16-5632074449aa.png" />
  <p align="center">
  <a href="https://nodejs.org/en/">
    <img src="https://img.shields.io/badge/-NodeJS-006400?style=flat&logo=Node.js&logoColor=#339933" />
  </a>
  <a href="https://pt-br.reactjs.org/">
     <img src="https://img.shields.io/badge/-React-1AB7EA?style=flat&logo=React&logoColor=#61DAFB" />
  </a>
  <a href="https://reactnative.dev/">
     <img src="https://img.shields.io/badge/-React Native-1AB7EA?style=flat&logo=React&logoColor=#61DAFB" />
  </a>
  <a href="https://www.typescriptlang.org/">
    <img src="https://img.shields.io/badge/-TypeScript-007ACC?style=flat&logo=TypeScript&logoColor=#007ACC" />
  </a>
  <a href="https://github.com/Rocketseat">
    <img src="https://img.shields.io/badge/-RocketSeat-7C4EC4?style=flat&logo=Apache%20RocketMQ&logoColor=FFF" />
  </a>
  </p>
</h1>

## 🔖 Sobre o projeto 

O projeto **gobarber** desenvolvido durante as aulas do bootcamp da [Rocktseat](https://rocketseat.com.br/ "Rocktseat"), com o intuito de achar barbeiros para marcação de agendamentos.

- **Features**
  - Cadastros - ✅
  - Login/Logout - ✅
  - Busca de barbeiros/cabeleleiros - ✅
  - Marcação de agendamento - ✅

Versões: 
  - **Web** 🖥  - Finalizada ✅  
  - **Mobile** 📱 - em progresso 🕐

## 💻 Tecnologias 

- **Backend** ⚙️
  - <img width="20px" src="https://img.icons8.com/color/2x/nodejs.png" /> [NodeJS](https://nodejs.org/en/ "NodeJS")
  - <img width="20px" src="https://img.icons8.com/color/2x/typescript.png" /> [TypeScript](https://www.typescriptlang.org/ "TypeScript")
  - <img width="20px" src="https://res.cloudinary.com/practicaldev/image/fetch/s--00h6CjGb--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://www.maxrooted.com/panduan-membangun-rest-api-expressjs-mysql/cover.png" /> [Express](https://expressjs.com/ "Express")
  - <img width="20px" src="https://img.icons8.com/color/2x/postgreesql.png" /> [PostgreSQL](https://www.postgresql.org/ "PostgreSQL")
  - <img width="20px" src="https://img.icons8.com/color/2x/mongodb.png" /> [MongoDB](https://www.mongodb.com/ "MongoDB") - Utilizado para notificações
  - <img width="20px" src="https://img.icons8.com/color/2x/redis.png" /> [Redis](https://redis.io/ "Redis") - Utilizado para cache
  - <img width="20px" src="https://avatars2.githubusercontent.com/u/20165699?s=400&v=4" /> [TypeORM](https://typeorm.io/#/ "TypeORM") - Framework para queries
  - <img width="20px" src="https://img.icons8.com/dusk/2x/docker.png" /> [Docker](https://www.docker.com/ 'Docker')
 
- **Frontend** 🖼
  - <img width="20px" src="https://img.icons8.com/color/2x/react-native.png" /> [React Native](https://reactnative.dev/ "React Native") - **mobile**
  - <img width="20px" src="https://img.icons8.com/plasticine/2x/react.png" /> [React JS ](https://pt-br.reactjs.org/ "React JS ") - **web**
  - <img width="20px" src="https://img.icons8.com/color/2x/typescript.png" /> [TypeScript](https://www.typescriptlang.org/ "TypeScript")
  - <img width="20px" src="https://styled-components.com/logo.png" /> [Styled Components](https://styled-components.com/ "Styled Components")
  - <img width="20px" src="https://img.icons8.com/dotty/2x/numbers-input-form.png" /> [Unform](https://github.com/Rocketseat/unform "Unform") - **Validação de forms**
  - <img width="20px" src="https://img.icons8.com/office/2x/password-check.png" /> [Yup](https://www.npmjs.com/package/yup "Yup") - **Validação de campos**
 
## ▶️ Getting Started 

 - **Passo 1️⃣** : git clone do projeto [GoBarber](https://github.com/rafaelsanzio/gostack-gobarber "GoBarber")

- **Backend** ⚙️

  - **Passo 1️⃣** : executar a instalação do [NodeJS](https://nodejs.org/en/ "NodeJS") e [Docker](https://www.docker.com/ "Docker")
  ```bash
    # Navegando até a pasta do backend do projeto
    $ cd gostack-gobarber/backend

    # Instalando todas as depêndencias necessárias
    $ npm install || yarn install
    
    # Criando container para o banco de dados PostgreSQL usando o docker
    $ docker run --name gobarber_db -e POSTGRES_PASSWORD=gobarber -p 5432:5432 -d postgres
    
    # Iniciando o banco de dados
    $ docker start gobarber_db
    
    # Criando cluster no banco de dados mongoDB usando o docker para notificações
    $ docker run --name mongodb -p 27017:27017 -d -t mongo

    # Iniciando o banco de dados mongo 
    $ docker start mongodb
    
    # Criando imagem banco de dados redis para cache da aplicação
    $ docker run --name redis -p 6379:6379 -d -t redis:alpine
    
    # Iniciando o banco de dados redis 
    $ docker start redis

    # Starting o backend da aplicação
    $ npm dev:server ou yarn dev:server
    ```

- **Frontend** 🖼

  - **Web** 💻

	 ```bash
    # Navegando até a pasta do projeto
    $ cd gostack-gobarber/web

    # Instalando todas as depêndencias necessárias
    $ npm install ou yarn install

    # Starting o frontend web da aplicação
    $ npm start ou yarn start
	 ```

  - **Mobile** 📱

	 ```bash
    # Navegando até a pasta do projeto
    $ cd gostack-gobarber/mobile

    # Instalando todas as depêndencias necessárias
    $ npm install ou yarn install

    # Starting o frontend mobile da aplicação
    iOS - $ yarn ios
    Android - $ yarn android
	 ```

## 📸 Imagens

 <p align="center">
 	<img src="https://user-images.githubusercontent.com/18368947/87234474-b01f0880-c3a7-11ea-80a4-a6edd5498e0d.png" />
 </p>
 
 - [Layout GoBarber](https://www.figma.com/file/BXCihtXXh9p37lGsENV614/GoBarber?node-id=0%3A1)

## ㊗️ Considerações 
- Projeto desenvolvido no Bootcamp - GoStack da [RocketSeat](https://rocketseat.com.br/ "RocketSeat")  by:

  - <a href="https://github.com/rafaelsanzio">
    <img src="https://img.shields.io/badge/-Rafael%20Sanzio-000000?style=flat&logo=GitHub&logoColor=#000000" />
  </a>

  - <a href="https://www.linkedin.com/in/rafael-sanzio-012778143/">
    <img src="https://img.shields.io/badge/-Rafael%20Sanzio-0077B5?style=flat&logo=LinkedIN&logoColor=#000000" />
  </a>




