# Backend com NestJS, Docker e Prisma

Este projeto é um servidor backend desenvolvido com NestJS, utilizando Docker para criar um ambiente de desenvolvimento consistente e Prisma como ORM para gerenciar o banco de dados.

## Instalação

Para instalar, comece clonando este repositório em sua máquina local:

````bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

```bash
yarn install

# Edite o arquivo .env com suas configurações
```bash
cp .env.example .env

# Com o Docker instalado, execute o comando abaixo para iniciar os serviços do Docker:
```bash
docker-compose up -d

#Após isso, aplique as migrações do Prisma para criar as tabelas no banco de dados:
```bash
yarn prisma migrate dev

#Por fim, inicie o servidor de desenvolvimento do NestJS com o comando:
```bash
yarn start:dev



# NestJs Jwt Authentication with access token and refresh token - Integration and End-to-end tests included

This is an example of how to implement an authentication system in NestJs using passport.js, and json web tokens (JWT).

I've included integration tests in the auth module under "test" folder.

The e2e tests on the other hand are in the root test folder.

```bash
yarn test # run integration test
yarn test:e2e # run e2e tests
````
