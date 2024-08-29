# Backend com NestJS, Docker e Prisma

This project is a backend server developed with NestJS, using Docker to create a consistent development environment and Prisma as the ORM to manage the database.

## Installation

To install, start by cloning this repository to your local machine:

```bash
git clone https://github.com/carlosedrocha/condominium-management-api.git
cd your-repository
```

Then, install the dependencies:

```bash
yarn
```

Next, edit the `.env` file with your configurations:

```bash
cp .env.example .env
```

With Docker installed, run the following command to start the Docker services:

```bash
docker-compose up -d
```

After that, apply the Prisma migrations to create the tables in the database:

```bash
npx prisma migrate dev
```

Finally, start the NestJS development server with the following command:

```bash
yarn start:dev
```

## NestJs Jwt Authentication with access token and refresh token - Integration and End-to-end tests included

This is an example of how to implement an authentication system in NestJs using passport.js and JSON web tokens (JWT).

Integration tests are included in the `test` folder under the auth module.

The end-to-end tests are located in the root `test` folder.

To run the integration tests, use the following command:

```bash
yarn test
```

To run the end-to-end tests, use the following command:

```bash
yarn test:e2e
```
