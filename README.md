<h1 align="center">
    <!-- Logo da Aplicação -->
    <img alt="Logo" src=".github/logo_gobarber.png" width="200px"/>
    <p>GoBarber API</p>
</h1>

<h3 align="center">
    <!-- Descrição do projeto  -->
    Beauty service scheduling system - REST API built with Node.js
</h3>
</br>
<div align="center">

[![](https://img.shields.io/badge/made%20by-ThiagoGualberto-%237159C1)](https://www.linkedin.com/in/thiago-medeiros-7478816b/)
[![](https://img.shields.io/badge/node.js@lts-12.14.1-informational?logo=Node.JS)](https://github.com/nodejs/node/blob/master/doc/changelogs/CHANGELOG_V12.md#12.14.1)
![](https://img.shields.io/github/languages/top/thiagogualberto/gobarber-api.svg?color=yellow)
![](https://img.shields.io/github/languages/count/thiagogualberto/gobarber-api.svg?color=lightgrey)
[![](https://api.codacy.com/project/badge/Grade/764eee83d7604873a9b06d37c4689523)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=DanielObara/DesafioFastFeet&amp;utm_campaign=Badge_Grade)
![](https://img.shields.io/github/repo-size/thiagogualberto/gobarber-api.svg)
[![GitHub last commit](https://img.shields.io/github/last-commit/thiagogualberto/gobarber-api.svg?color=red)](https://github.com/thiagogualberto/gobarber-api/commits/master)
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/thiagogualberto/gobarber-api/blob/master/LICENSE)

</div>
<p align="center">
  <a href="#man_technologist-project">Project</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#rocket-getting-started">Getting Started</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#clipboard-features">Features</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#thinking-contribution">Contribution</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#pushpin-support">Support</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licenca">Licença</a>
</p>
</br>

# 👨🏻‍💻 :man_technologist: Project

This project is a challenge of Rocketseat GoStack Bootcamp. It's a REST API built with NodeJS + Express. This API is a beauty service scheduling system that connects clients and providers.

# :rocket: Getting Started

## ⚙️ Back-end

To clone and run this api, you'll need Git, Node.js v12.14 or higher + Yarn v1.21 or higher + Docker installed on your computer. </br>
The first thing you need to do is to run these three containers on your machine:</br>

```bash
# Create a container in 'postgres' with the name of 'database'
$ docker run --name database -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres

#Create a container in 'mongo' with the name of 'mongobarber'
$ docker run --name mongobarber -p 27017:27017 -d -t mongo

# Create a container in 'redis' with the name of 'redisbarber'
$ docker run --name redisbarber -p 6379:6379 -d -t redis:alpine
```
</br>From your command line:

```bash
# Clone this repo to your local machine using
$ git clone https://github.com/thiagogualberto/gobarber-api.git

# From the project root, enter the backend (gobarber-api) folder
$ cd gobarber-api

# Install the dependencies
$ yarn

# Create a database in 'postgres' with the name of 'gobarber';

# Make a copy of the .env.example file to .env and fill it with YOUR variables.
$ cp .env.example .env

# Run the migrations
$ yarn sequelize db:migrate

# Everything ready to start the server
$ yarn dev
```

Importe o arquivo `Insomnia.json` no Insomnia ou clique no botão [Run in Insomnia](#insomniaButton)

---

# 📋 :clipboard: Features
## Funcionalities
- User authentication with JWT
- User registration (Create, Read, Update and Delete)
- Sending files (User avatar)
- Schedules
    - List of service providers
    - Service scheduling
    - Validation of appointments
    - Listing user schedules
    - Pagination
    - Listing provider's agenda
- Sending notifications
    - Notifying new appointments
    - Listing user notifications
    - Mark notifications as read
- Cancellation and sending email
    - Cancellation of scheduling
    - Listing available times

## Build with (Technologies)

This project was developed with the following technologies:
- [Bcrypt](https://www.npmjs.com/package/bcrypt) - Generation of User Password Hash
- [Bee Queue](https://github.com/bee-queue/bee-queue) - Redis-backed job queue for Node.js.
- [date-fns](https://date-fns.org/) - JavaScript date utility library
- [Docker](https://www.docker.com/docker-community) - Container
- [DotEnv](https://www.npmjs.com/package/dotenv) - Loads environment variables
- [EditorConfig](https://editorconfig.org/) - Setting up the development environment
- [ESLint](https://eslint.org/) - JS Linter and code style
- [Express](https://expressjs.com/pt-br/) - Router of the Application
- [JWT](https://jwt.io/) - Authentication Json Web Token
- [MongoDB](https://www.mongodb.com/) - Database
- [Mongoose](https://mongoosejs.com/) - Object Modeling + DB Connector
- [Multer](https://github.com/expressjs/multer) - File Upload
- [Nodemailer](https://nodemailer.com/about/) - Used to send emails
- [Nodemon](https://nodemon.io/) - Process Manager used in the development
- [Node.js](https://nodejs.org/en/) - Build the server
- [PostgreSQL](https://www.postgresql.org/) - Database
- [Prettier](https://prettier.io/) - Code Formatter
- [Sequelize](https://sequelize.org/) - Promise-based Node.js ORM for Postgres
- [Sucrase](https://github.com/alangpierce/sucrase) - Setting up the development environment
- [VS Code](https://code.visualstudio.com/) with [Sucrase](https://github.com/alangpierce/sucrase) + [Nodemon](https://nodemon.io/) + [ESLint](https://eslint.org/) + [Prettier](https://prettier.io/) + [EditorConfig](https://editorconfig.org/) + [Sequelize](https://sequelize.org/)
- [Youch](https://www.npmjs.com/package/youch)
- [Yup](https://www.npmjs.com/package/yup) - Validate the application's JSON fields.

# 🤔 :thinking: Contribution

I'll be happy if you could provide me any feedback about the project, code, structure or anything that you can report that could make me a better developer!

```bash
#Fork this repo!
$ gh repo fork thiagogualberto/NOME_DO_REPO

#Clone this repo to your local machine using
$ git clone https://github.com/thiagogualberto/gobarber-api.git

# Create your feature branch using
$ git checkout -b my-feature

# Commit your changes using
$ git commit -m 'feat: My new feature'

# Push to the branch using
$ git push origin my-feature

# Create a new pull request

After your Pull Request is merged, can you delete your feature branch.
```

You can send how many PR's do you want, I'll be glad to analyse and accept them! And if you have any question about the project contact me by email or linkedin below and let's have a good chat.

---


# 📌 :pushpin: Support
My name is Thiago de Medeiros Gualberto and my contacts are:

- Email: thiago.gou@gmail.com
- Linkedin at [Thiago Medeiros](https://www.linkedin.com/in/thiago-medeiros-7478816b/)

Connect with me at LinkedIn.

Thank you!

# 📝 :memo: Licença

[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/thiagogualberto/gobarber-api/blob/master/LICENSE)

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details


---
Made with ♥ Enjoy it!
