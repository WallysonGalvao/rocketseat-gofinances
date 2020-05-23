<h1 align="center">
    <img alt="GoFinances" title="#delicinha" src="../.github/logo.svg" width="250px" />
</h1>

<p align="center">
  <a href="#rocket-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#collision-funcionalidades">Funcionalidades</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#zap-rodando-o-projeto">Rodando o Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#notebook-enpoints">Endpoints</a>
</p>

<h2>
<strong>Backend</strong> da aplicação GoFinances.
</h2>

## :rocket: Tecnologias

### **Ferramentas usadas**

- Express
- JWT + Bcryptjs
- ESLint + Prettier + EditorConfig;
- TypeORM + PostgreSQL;

## :collision: Funcionalidades

Abaixo estão descritas as funcionalidades para o administrador e os entregadores da aplicação:

### **Administrador**

### 1. Autenticação

Autenticação do usuário administrador com e-mail e senha.

### 2. Gestão Financeira

Inserir entrada e saída de dinheiro.

## :zap: Rodando o projeto

### Docker

1 - É preciso ter o [Docker](https://www.docker.com/) instaldo em sua máquina. Feito a instalação, rodar os seguintes comandos:

```
$ docker run --name database -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
$ docker run --name redisgofinances -p 6379:6379 -d -t redis:alpine
```

2 - Após executar os comandos acima, verificar se as imagens estão rodando no terminal:

```
$ docker ps
```

3 - Caos as imagens estejam paradas/não aparecer no terminal, executar:

```
$ docker start database
$ docker start redisgofinances
```

### Backend

1 - Em um terminal, entrar na raiz do projeto **/backend** e rodar o comando:

```
$ yarn install
```

2 - Ainda na raiz do projeto, rodar em abas diferentes os comandos:

```
$ yarn dev
```

Feito isso, acessar o endereço http://localhost:3333

## :notebook: Endpoints

Você pode executar online ou fazer o download dos endpoints e executar diretamente no Insomnia:

[![Run in Insomnia}](https://insomnia.rest/images/run.svg)](https://insomnia.rest/run/?label=&uri=https%3A%2F%2Fraw.githubusercontent.com%2FWallysonGalvao%2Frocketseat-gofinances%2Fmaster%2Fbackend%2Fendpoints.json)

---
