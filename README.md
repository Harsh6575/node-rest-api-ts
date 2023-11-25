# The Complete Guide To Building A REST API With Node, Express, TypeScript & MongoDB

This is a repository for a REST API tutorial using Node, Express, Typescript & MongoDB.

Features:

- Environment, Typescript, Nodemon setup
- MongoDB & Mongoose connect, Database creation
- Controllers creation
- Middlewares creation
- Cookie based authentication
- Postman testing
- Create, Read, Update

### Prerequisites

**Node version 14.x**

### Install packages

```shell
npm i
```

### Setup MongoDB URL

In `src/index.ts`:

```js
const MONGO_URL = ''; // DB URI
```

### Start the app

```shell
npm start
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `start`         | Starts a development instance of the app |

## Api Test AUTH (POST REQ)

| api         |input                              |
| :-------------- | :--------------------------------------- |
| `http://localhost:8080/auth/register`         | { "email": "dummy@gmail.com", "username":"Dummy", "password":"HPpatel" } |
| `http://localhost:8080/auth/login`         | { "email": "dummy@gmail.com", "password":"HPpatel" } |

## Api Test USERS

| api         |req type                              | data |
| :-------------- | :--------------------------------------- |:---|
| `http://localhost:8080/users`         | GET |
| `http://localhost:8080/users/[id]`         | DELETE |
| `http://localhost:8080/users/[id]`         | PATCH |  {"username": "MODIFIEDHARSH"}|